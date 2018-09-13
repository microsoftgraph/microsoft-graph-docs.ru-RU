# <a name="managedappdataencryptiontype-enum-type"></a><span data-ttu-id="8357f-101">тип перечисления managedAppDataEncryptionType</span><span class="sxs-lookup"><span data-stu-id="8357f-101">managedAppDataEncryptionType enum type</span></span>

> <span data-ttu-id="8357f-102">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="8357f-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="8357f-103">Представляет уровень, для которого данные приложения шифруются для управляемых приложений</span><span class="sxs-lookup"><span data-stu-id="8357f-103">Represents the level to which app data is encrypted for managed apps</span></span>
## <a name="members"></a><span data-ttu-id="8357f-104">Элементы</span><span class="sxs-lookup"><span data-stu-id="8357f-104">Members</span></span>
|<span data-ttu-id="8357f-105">Элемент</span><span class="sxs-lookup"><span data-stu-id="8357f-105">Member</span></span>|<span data-ttu-id="8357f-106">Значение</span><span class="sxs-lookup"><span data-stu-id="8357f-106">Value</span></span>|<span data-ttu-id="8357f-107">Описание</span><span class="sxs-lookup"><span data-stu-id="8357f-107">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8357f-108">useDeviceSettings</span><span class="sxs-lookup"><span data-stu-id="8357f-108">useDeviceSettings</span></span>|<span data-ttu-id="8357f-109">0</span><span class="sxs-lookup"><span data-stu-id="8357f-109">0%</span></span>|<span data-ttu-id="8357f-110">Данные приложения шифруются на основе параметров по умолчанию на устройстве.</span><span class="sxs-lookup"><span data-stu-id="8357f-110">App data is encrypted based on the default settings on the device.</span></span>|
|<span data-ttu-id="8357f-111">afterDeviceRestart</span><span class="sxs-lookup"><span data-stu-id="8357f-111">afterDeviceRestart</span></span>|<span data-ttu-id="8357f-112">1</span><span class="sxs-lookup"><span data-stu-id="8357f-112">-1</span></span>|<span data-ttu-id="8357f-113">Данные приложения шифруются при перезапуске устройства.</span><span class="sxs-lookup"><span data-stu-id="8357f-113">App data is encrypted when the device is restarted.</span></span>|
|<span data-ttu-id="8357f-114">whenDeviceLockedExceptOpenFiles</span><span class="sxs-lookup"><span data-stu-id="8357f-114">whenDeviceLockedExceptOpenFiles</span></span>|<span data-ttu-id="8357f-115">2</span><span class="sxs-lookup"><span data-stu-id="8357f-115">2</span></span>|<span data-ttu-id="8357f-116">Данные приложения, связанные с этой политикой, шифруются при блокировке устройства, за исключением данных в открытых файлах</span><span class="sxs-lookup"><span data-stu-id="8357f-116">App data associated with this policy is encrypted when the device is locked, except data in files that are open</span></span>|
|<span data-ttu-id="8357f-117">whenDeviceLocked</span><span class="sxs-lookup"><span data-stu-id="8357f-117">whenDeviceLocked</span></span>|<span data-ttu-id="8357f-118">3</span><span class="sxs-lookup"><span data-stu-id="8357f-118">3</span></span>|<span data-ttu-id="8357f-119">Данные приложения, связанные с этой политикой, шифруются при блокировке устройства</span><span class="sxs-lookup"><span data-stu-id="8357f-119">App data associated with this policy is encrypted when the device is locked</span></span>|








