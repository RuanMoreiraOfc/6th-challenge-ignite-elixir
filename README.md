<h1 align='center'>
6th Challenge Elixir
</h1>

This repo includes the resolution for 6th Challenge in Elixir Journey with [Rafael Camada][btn-tutor].

## GOAL

```elixir
params1 = %{
  complete_date: ~N[2021-03-22 19:29:25.607218],
  local_origin: "Vitória",
  local_destination: "Salvador",
  user_id: "user_id1",
  id: UUID.uuid4()
}
params2 = %{
  complete_date: ~N[2021-03-14 12:12:25.607218],
  local_origin: "São Paulo",
  local_destination: "Rio de Janeiro",
  user_id: "user_id2",
  id: UUID.uuid4()
}
params3 = %{
  complete_date: ~N[2021-04-18 08:45:25.607218],
  local_origin: "São Paulo",
  local_destination: "Londres",
  user_id: "user_id3",
  id: UUID.uuid4()
}

Flightex.start_agents()
Flightex.create_or_update_booking(params1)
Flightex.create_or_update_booking(params2)
Flightex.create_or_update_booking(params3)
Flightex.generate_report(from_date, to_date)
```

```elixir
# report.csv
user_id1,Vitória,Salvador,2021-03-22 19:29:25.607218
user_id2,São Paulo,Rio de Janeiro,2021-03-14 12:12:25.607218
user_id3,São Paulo,Londres,2021-04-18 08:45:25.607218
```

<!-- VARIABLES -->

[btn-tutor]: https://github.com/rafaelcamarda
