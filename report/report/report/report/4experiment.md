print("Process | AT | BT | PR | ST | CT | TAT | WT")
print("-" * 50)

for p in processes:
    print(f"{p.name:^7} | {p.arrival_time:^2} | {p.burst_time:^2} | "
          f"{p.priority:^2} | {p.start_time:^2} | {p.completion_time:^2} | "
          f"{p.turnaround_time:^3} | {p.waiting_time:^2}")

