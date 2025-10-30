## 1.Debloat Win11 and Setup
https://github.com/Raphire/Win11Debloat
https://github.com/ChrisTitusTech/winutil
Disable Defender ( Broke MS Store)
https://github.com/lostzombie/AchillesScript

## 2.Debloat Nvidia Driver
https://www.techpowerup.com/download/techpowerup-nvcleanstall/

## 3.Setup MSI Mode and GPU Affinity
https://github.com/valleyofdoom/AutoGpuAffinity

## 4. NV Inspector Tweaks

## 5. Bcdedit 
Dynamic Tick Rate disable

## 6.LAN
NDIS Realtek 2.5Gb Driver Support RSS
NetAdapterCx didnt Support it



https://signalrgb.com/
https://github.com/zinzied/Windows-11-Manager

## IRQ Tweak
Although this step may have been caried out in an earlier section to rule out the hardware-related causes of IRQ sharing, the software-related causes of potential IRQ sharing can be assessed now by confirming that there is no IRQ sharing on your system by typing msinfo32 in Win+R then navigating to the Conflicts/Sharing section

If the System timer device and High precision event timer are sharing IRQ 0, a solution to this is to disable the parent device's driver of System timer which is PCI standard ISA bridge. This can be accomplished with the command below. It is important to note that disabling msisadrv breaks the keyboard on mobile devices 

`reg add "HKLM\SYSTEM\CurrentControlSet\Services\msisadrv" /v "Start" /t REG_DWORD /d "4" /f`

https://www.reddit.com/r/OptimizedGaming/comments/1j6qdgb/guide_changing_display_topology_to_reduce_monitor/

https://donewmouseaccel.blogspot.com/
