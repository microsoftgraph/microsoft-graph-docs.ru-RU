# <a name="delete-ioslobapp"></a><span data-ttu-id="ce457-101">Удаление объекта iosLobApp</span><span class="sxs-lookup"><span data-stu-id="ce457-101">Delete iosLobApp</span></span>

> <span data-ttu-id="ce457-102">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="ce457-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="ce457-103">Удаляет объект [iosLobApp](../resources/intune_apps_ioslobapp.md).</span><span class="sxs-lookup"><span data-stu-id="ce457-103">Deletes a [iosLobApp](../resources/intune_apps_ioslobapp.md).</span></span>
## <a name="prerequisites"></a><span data-ttu-id="ce457-104">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="ce457-104">Prerequisites</span></span>
<span data-ttu-id="ce457-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="ce457-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="ce457-107">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ce457-107">Permission type</span></span>|<span data-ttu-id="ce457-108">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="ce457-108">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ce457-109">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ce457-109">Delegated (work or school account)</span></span>|<span data-ttu-id="ce457-110">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ce457-110">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="ce457-111">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ce457-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ce457-112">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ce457-112">Not supported.</span></span>|
|<span data-ttu-id="ce457-113">Для приложений</span><span class="sxs-lookup"><span data-stu-id="ce457-113">Application</span></span>|<span data-ttu-id="ce457-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ce457-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="ce457-115">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ce457-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /deviceAppManagement/mobileApps/{mobileAppId}
```

## <a name="request-headers"></a><span data-ttu-id="ce457-116">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="ce457-116">Request headers</span></span>
|<span data-ttu-id="ce457-117">Заголовок</span><span class="sxs-lookup"><span data-stu-id="ce457-117">Header</span></span>|<span data-ttu-id="ce457-118">Значение</span><span class="sxs-lookup"><span data-stu-id="ce457-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ce457-119">Авторизация</span><span class="sxs-lookup"><span data-stu-id="ce457-119">Authorization</span></span>|<span data-ttu-id="ce457-120">&lt;Токен&gt; носителя. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="ce457-120">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="ce457-121">Принять</span><span class="sxs-lookup"><span data-stu-id="ce457-121">Accept</span></span>|<span data-ttu-id="ce457-122">application/json</span><span class="sxs-lookup"><span data-stu-id="ce457-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ce457-123">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="ce457-123">Request body</span></span>
<span data-ttu-id="ce457-124">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="ce457-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ce457-125">Отклик</span><span class="sxs-lookup"><span data-stu-id="ce457-125">Response</span></span>
<span data-ttu-id="ce457-126">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="ce457-126">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="ce457-127">Пример</span><span class="sxs-lookup"><span data-stu-id="ce457-127">Example</span></span>
### <a name="request"></a><span data-ttu-id="ce457-128">Запрос</span><span class="sxs-lookup"><span data-stu-id="ce457-128">Request</span></span>
<span data-ttu-id="ce457-129">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="ce457-129">Here is an example of the request.</span></span>
``` http
DELETE https://graph.microsoft.com/v1.0/deviceAppManagement/mobileApps/{mobileAppId}
```

### <a name="response"></a><span data-ttu-id="ce457-130">Ответ</span><span class="sxs-lookup"><span data-stu-id="ce457-130">Response</span></span>
<span data-ttu-id="ce457-p102">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="ce457-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```



