# Unlock-CPU-in-Ubuntu
CPU limited ( Lock ) to 798 MHz

<p>In Windows Unclock with "ThrottleStop"</p>
<p>In Ubuntu Unlock with this Script</p>

  

<p>Voici un code en C :</p>

<pre><code>
    # Resolve problem cpu Lock in ubuntu
    # Need :
    # sudo apt-get install cpufrequtils
    # sudo apt-get install msr-tools

    sudo cpufreq-set -c 0 -g performance
    sudo cpufreq-set -c 1 -g performance
    sudo cpufreq-set -c 2 -g performance
    sudo cpufreq-set -c 3 -g performance
    sudo modprobe msr
    sudo wrmsr 0x1FC 17422
</code></pre>
