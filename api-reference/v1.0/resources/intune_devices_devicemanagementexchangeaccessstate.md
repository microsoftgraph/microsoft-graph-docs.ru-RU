# <a name="devicemanagementexchangeaccessstate-enum-type"></a><span data-ttu-id="727ab-101">Тип перечисления deviceManagementExchangeAccessState</span><span class="sxs-lookup"><span data-stu-id="727ab-101">deviceManagementExchangeAccessState enum type</span></span>

> <span data-ttu-id="727ab-102">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="727ab-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="727ab-103">Состояние доступа к Exchange для устройств.</span><span class="sxs-lookup"><span data-stu-id="727ab-103">Device Exchange Access State summary</span></span>
## <a name="members"></a><span data-ttu-id="727ab-104">Элементы</span><span class="sxs-lookup"><span data-stu-id="727ab-104">Members</span></span>
|<span data-ttu-id="727ab-105">Элемент</span><span class="sxs-lookup"><span data-stu-id="727ab-105">Member</span></span>|<span data-ttu-id="727ab-106">Значение</span><span class="sxs-lookup"><span data-stu-id="727ab-106">Value</span></span>|<span data-ttu-id="727ab-107">Описание</span><span class="sxs-lookup"><span data-stu-id="727ab-107">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="727ab-108">none</span><span class="sxs-lookup"><span data-stu-id="727ab-108">none</span></span>|<span data-ttu-id="727ab-109">0</span><span class="sxs-lookup"><span data-stu-id="727ab-109">0%</span></span>|<span data-ttu-id="727ab-110">Состояние доступа к Exchange не определено</span><span class="sxs-lookup"><span data-stu-id="727ab-110">No access state discovered from Exchange</span></span>|
|<span data-ttu-id="727ab-111">unknown</span><span class="sxs-lookup"><span data-stu-id="727ab-111">unknown</span></span>|<span data-ttu-id="727ab-112">1</span><span class="sxs-lookup"><span data-stu-id="727ab-112">-1</span></span>|<span data-ttu-id="727ab-113">Состояние доступа устройства к Exchange неизвестно</span><span class="sxs-lookup"><span data-stu-id="727ab-113">Device access state to Exchange is unknown</span></span>|
|<span data-ttu-id="727ab-114">allowed</span><span class="sxs-lookup"><span data-stu-id="727ab-114">Allowed</span></span>|<span data-ttu-id="727ab-115">2</span><span class="sxs-lookup"><span data-stu-id="727ab-115">2</span></span>|<span data-ttu-id="727ab-116">У устройства есть доступ к Exchange</span><span class="sxs-lookup"><span data-stu-id="727ab-116">Device has access to Exchange</span></span>|
|<span data-ttu-id="727ab-117">blocked</span><span class="sxs-lookup"><span data-stu-id="727ab-117">blocked</span></span>|<span data-ttu-id="727ab-118">3</span><span class="sxs-lookup"><span data-stu-id="727ab-118">3</span></span>|<span data-ttu-id="727ab-119">Устройство заблокировано в Exchange</span><span class="sxs-lookup"><span data-stu-id="727ab-119">Device is Blocked in Exchange</span></span>|
|<span data-ttu-id="727ab-120">quarantined</span><span class="sxs-lookup"><span data-stu-id="727ab-120">quarantined</span></span>|<span data-ttu-id="727ab-121">4</span><span class="sxs-lookup"><span data-stu-id="727ab-121">4</span></span>|<span data-ttu-id="727ab-122">Устройство находится в карантине Exchange</span><span class="sxs-lookup"><span data-stu-id="727ab-122">Device is Quarantined in Exchange</span></span>|








