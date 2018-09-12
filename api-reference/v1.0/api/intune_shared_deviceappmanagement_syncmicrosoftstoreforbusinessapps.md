# <a name="syncmicrosoftstoreforbusinessapps-action"></a><span data-ttu-id="95c8c-101">Действие syncMicrosoftStoreForBusinessApps</span><span class="sxs-lookup"><span data-stu-id="95c8c-101">syncMicrosoftStoreForBusinessApps action</span></span>

> <span data-ttu-id="95c8c-102">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="95c8c-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="95c8c-103">Синхронизирует учетную запись Intune с Microsoft Store для бизнеса</span><span class="sxs-lookup"><span data-stu-id="95c8c-103">Syncs Intune account with Microsoft Store For Business</span></span>
## <a name="prerequisites"></a><span data-ttu-id="95c8c-104">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="95c8c-104">Prerequisites</span></span>
<span data-ttu-id="95c8c-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="95c8c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="95c8c-107">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="95c8c-107">Permission type</span></span>|<span data-ttu-id="95c8c-108">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="95c8c-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="95c8c-109">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="95c8c-109">Delegated (work or school account)</span></span>| 
| <span data-ttu-id="95c8c-110">&nbsp; &nbsp; _Адаптация_</span><span class="sxs-lookup"><span data-stu-id="95c8c-110">&nbsp; &nbsp; _On-boarding_</span></span> | <span data-ttu-id="95c8c-111">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="95c8c-111">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="95c8c-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="95c8c-112">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="95c8c-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="95c8c-113">Not supported.</span></span>|
|<span data-ttu-id="95c8c-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="95c8c-114">Application</span></span>|<span data-ttu-id="95c8c-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="95c8c-115">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="95c8c-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="95c8c-116">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/syncMicrosoftStoreForBusinessApps
```

## <a name="request-headers"></a><span data-ttu-id="95c8c-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="95c8c-117">Request headers</span></span>
|<span data-ttu-id="95c8c-118">Заголовок</span><span class="sxs-lookup"><span data-stu-id="95c8c-118">Header</span></span>|<span data-ttu-id="95c8c-119">Значение</span><span class="sxs-lookup"><span data-stu-id="95c8c-119">Value</span></span>|
|:---|:---|
|<span data-ttu-id="95c8c-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="95c8c-120">Authorization</span></span>|<span data-ttu-id="95c8c-121">Требуется Bearer &lt;маркер&gt;</span><span class="sxs-lookup"><span data-stu-id="95c8c-121">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="95c8c-122">Принять</span><span class="sxs-lookup"><span data-stu-id="95c8c-122">Accept</span></span>|<span data-ttu-id="95c8c-123">application/json</span><span class="sxs-lookup"><span data-stu-id="95c8c-123">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="95c8c-124">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="95c8c-124">Request body</span></span>
<span data-ttu-id="95c8c-125">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="95c8c-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="95c8c-126">Ответ</span><span class="sxs-lookup"><span data-stu-id="95c8c-126">Response</span></span>
<span data-ttu-id="95c8c-127">В случае успешного выполнения это действие возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="95c8c-127">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example-request"></a><span data-ttu-id="95c8c-128">Пример запроса</span><span class="sxs-lookup"><span data-stu-id="95c8c-128">Example request</span></span>

``` http
POST https://graph.microsoft.com/v1.0/deviceAppManagement/syncMicrosoftStoreForBusinessApps
```

### <a name="response"></a><span data-ttu-id="95c8c-129">Ответ</span><span class="sxs-lookup"><span data-stu-id="95c8c-129">Response</span></span>

<span data-ttu-id="95c8c-130">Представленный здесь объект отклика может быть усечен для краткости.</span><span class="sxs-lookup"><span data-stu-id="95c8c-130">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="95c8c-131">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="95c8c-131">All of the properties will be returned from an actual call.</span></span>

``` http
HTTP/1.1 204 No Content
```



