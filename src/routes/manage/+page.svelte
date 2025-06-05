<script>
	import { Button } from '$lib/components/ui/button';
	import { Input } from '$lib/components/ui/input';s
	import { z } from 'zod';
	export const fromSchema = z.object({
		username: z.string().min(2).max(50)
	});

	export type FormSchema = typeof fromSchema;
</script>
