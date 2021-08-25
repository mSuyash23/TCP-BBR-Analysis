# TCP-BBR-Analysis
For this project I've used the BBR implementation availabe here https://github.com/Vivek-anand-jain/Reproduce-TCP-BBR-in-ns-3
# What actually is TCP BBR Congestion control mechanism
TCP BBR Congestion control is designed to respond to actual congestion, rather than packet loss. The BBR team designed the algorithm with the desire to have something that responds to actual congestion, rather than packet loss. BBR models the network to send as fast as the available bandwidth and is 2700x faster than previous TCPs on a 10Gb, 100ms link with 1% loss

Focused on improving network performance when the network isn’t very good. TCP BBR more accurately balances fairness and utilization, resulting in better download speed over the same network. It’s most noticeable in situations where the network is bad (however, it doesn’t hurt you if you’re on a squeaky clean network)
Doesn’t require the client to implement BBR. This one is the magic pixie dust. Prior algorithms like QUIC required client & server to have both implemented the algorithm. BBR doesn’t require the client to be using BBR as well. This is especially relevant in the developing world which use older mobile platforms and have limited bandwidth, or areas where websites & services haven’t made the switch yet.

more details : https://medium.com/google-cloud/tcp-bbr-magic-dust-for-network-performance-57a5f1ccf437
for all the intricate details : https://dl.acm.org/doi/pdf/10.1145/3012426.3022184
