# <a name="devicemanagementexchangeconnectorsynctype-enum-type"></a><span data-ttu-id="952f6-101">Тип перечисления deviceManagementExchangeConnectorSyncType</span><span class="sxs-lookup"><span data-stu-id="952f6-101">deviceManagementExchangeConnectorSyncType enum type</span></span>

> <span data-ttu-id="952f6-102">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="952f6-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="952f6-103">Тип запрошенной синхронизации соединителя Exchange.</span><span class="sxs-lookup"><span data-stu-id="952f6-103">The type of Exchange Connector Configured.</span></span>
## <a name="members"></a><span data-ttu-id="952f6-104">Элементы</span><span class="sxs-lookup"><span data-stu-id="952f6-104">Members</span></span>
|<span data-ttu-id="952f6-105">Элемент</span><span class="sxs-lookup"><span data-stu-id="952f6-105">Member</span></span>|<span data-ttu-id="952f6-106">Значение</span><span class="sxs-lookup"><span data-stu-id="952f6-106">Value</span></span>|<span data-ttu-id="952f6-107">Описание</span><span class="sxs-lookup"><span data-stu-id="952f6-107">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="952f6-108">fullSync</span><span class="sxs-lookup"><span data-stu-id="952f6-108">fullSync</span></span>|<span data-ttu-id="952f6-109">0</span><span class="sxs-lookup"><span data-stu-id="952f6-109">0%</span></span>|<span data-ttu-id="952f6-110">Обнаружение всех устройств в Exchange.</span><span class="sxs-lookup"><span data-stu-id="952f6-110">Discover all the device in Exchange.</span></span>|
|<span data-ttu-id="952f6-111">deltaSync</span><span class="sxs-lookup"><span data-stu-id="952f6-111">deltaSync</span></span>|<span data-ttu-id="952f6-112">1</span><span class="sxs-lookup"><span data-stu-id="952f6-112">-1</span></span>|<span data-ttu-id="952f6-113">Обнаружение только тех устройств в Exchange, которые были обновлены во время окна дельта-синхронизации.</span><span class="sxs-lookup"><span data-stu-id="952f6-113">Discover only the device in Exchange which have updated during the delta sync window.</span></span>|








