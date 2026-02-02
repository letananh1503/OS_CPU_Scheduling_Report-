total_wt = 0
total_tat = 0

for p in processes:
    total_wt += p.waiting_time
    total_tat += p.turnaround_time

n = len(processes)
avg_wt = total_wt / n
avg_tat = total_tat / n

print(f"Average Waiting Time    = {avg_wt:.2f}")
print(f"Average Turnaround Time = {avg_tat:.2f}")
