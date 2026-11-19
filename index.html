-- Ejecutar en Supabase: SQL Editor > New query > Run
create table if not exists public.productos (
  id text primary key,
  nombre text not null,
  precios jsonb not null,      -- precios en soles, en el mismo orden que las presentaciones de la web
  disponible boolean not null default true
);
alter table public.productos enable row level security;
drop policy if exists "Todos pueden ver productos" on public.productos;
create policy "Todos pueden ver productos" on public.productos for select to anon using (true);
grant select on public.productos to anon;
-- Solo tú puedes modificar (desde Table Editor); los visitantes solo leen.
insert into public.productos (id, nombre, precios) values
 ('cheesecake-maracuya','Cheesecake de maracuyá','[12,60]'),
 ('cheesecake-copoazu','Cheesecake de copoazú','[12]'),
 ('tartaleta-camu-camu','Tartaleta de camu camu','[9]'),
 ('mousse-copoazu','Mousse de copoazú','[12]'),
 ('torta-aguaje','Torta de aguaje','[10,65]'),
 ('trufas-cocona','Trufas de cocona','[27]'),
 ('mousse-mango','Mousse de mango','[11]')
on conflict (id) do nothing;
-- Para cambiar un precio: Table Editor > productos > edita "precios" (ej. [13,60]).
-- Para marcar agotado: desmarca "disponible".
