# <a name="vpptokenstate-enum-type"></a><span data-ttu-id="4090c-101">Тип перечисления vppTokenState</span><span class="sxs-lookup"><span data-stu-id="4090c-101">vppTokenState enum type</span></span>

> <span data-ttu-id="4090c-102">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="4090c-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="4090c-103">Тип перечисления vppTokenState</span><span class="sxs-lookup"><span data-stu-id="4090c-103">Possible states associated with an Apple Volume Purchase Program token.</span></span>
## <a name="members"></a><span data-ttu-id="4090c-104">Элементы</span><span class="sxs-lookup"><span data-stu-id="4090c-104">Members</span></span>
|<span data-ttu-id="4090c-105">Элемент</span><span class="sxs-lookup"><span data-stu-id="4090c-105">Member</span></span>|<span data-ttu-id="4090c-106">Значение</span><span class="sxs-lookup"><span data-stu-id="4090c-106">Value</span></span>|<span data-ttu-id="4090c-107">Описание</span><span class="sxs-lookup"><span data-stu-id="4090c-107">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4090c-108">unknown</span><span class="sxs-lookup"><span data-stu-id="4090c-108">unknown</span></span>|<span data-ttu-id="4090c-109">0</span><span class="sxs-lookup"><span data-stu-id="4090c-109">0%</span></span>|<span data-ttu-id="4090c-110">Состояние по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="4090c-110">Default State</span></span>|
|<span data-ttu-id="4090c-111">valid</span><span class="sxs-lookup"><span data-stu-id="4090c-111">valid</span></span>|<span data-ttu-id="4090c-112">1</span><span class="sxs-lookup"><span data-stu-id="4090c-112">-1</span></span>|<span data-ttu-id="4090c-113">Маркер действителен.</span><span class="sxs-lookup"><span data-stu-id="4090c-113">Token is valid.</span></span>|
|<span data-ttu-id="4090c-114">expired</span><span class="sxs-lookup"><span data-stu-id="4090c-114">Expired</span></span>|<span data-ttu-id="4090c-115">2</span><span class="sxs-lookup"><span data-stu-id="4090c-115">2</span></span>|<span data-ttu-id="4090c-116">Срок действия маркера истек.</span><span class="sxs-lookup"><span data-stu-id="4090c-116">Token is expired.</span></span>|
|<span data-ttu-id="4090c-117">invalid</span><span class="sxs-lookup"><span data-stu-id="4090c-117">invalid</span></span>|<span data-ttu-id="4090c-118">3</span><span class="sxs-lookup"><span data-stu-id="4090c-118">3</span></span>|<span data-ttu-id="4090c-119">Маркер недействителен.</span><span class="sxs-lookup"><span data-stu-id="4090c-119">Token is invalid.</span></span>|
|<span data-ttu-id="4090c-120">assignedToExternalMDM</span><span class="sxs-lookup"><span data-stu-id="4090c-120">assignedToExternalMDM</span></span>|<span data-ttu-id="4090c-121">4</span><span class="sxs-lookup"><span data-stu-id="4090c-121">4</span></span>|<span data-ttu-id="4090c-122">Маркер управляется другой службой MDM.</span><span class="sxs-lookup"><span data-stu-id="4090c-122">Token is managed by another MDM Service.</span></span>|








