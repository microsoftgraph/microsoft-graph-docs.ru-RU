# <a name="renewupload-action"></a><span data-ttu-id="f79bc-101">Действие renewUpload</span><span class="sxs-lookup"><span data-stu-id="f79bc-101">renewUpload action</span></span>

> <span data-ttu-id="f79bc-102">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="f79bc-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="f79bc-103">Обновляет универсальный код ресурса SAS для отправки файла приложения.</span><span class="sxs-lookup"><span data-stu-id="f79bc-103">Renews the SAS URI for an application file upload.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="f79bc-104">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="f79bc-104">Prerequisites</span></span>
<span data-ttu-id="f79bc-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="f79bc-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="f79bc-107">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f79bc-107">Permission type</span></span>|<span data-ttu-id="f79bc-108">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="f79bc-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f79bc-109">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f79bc-109">Delegated (work or school account)</span></span>|<span data-ttu-id="f79bc-110">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f79bc-110">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="f79bc-111">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f79bc-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f79bc-112">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f79bc-112">Not supported.</span></span>|
|<span data-ttu-id="f79bc-113">Для приложений</span><span class="sxs-lookup"><span data-stu-id="f79bc-113">Application</span></span>|<span data-ttu-id="f79bc-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f79bc-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="f79bc-115">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f79bc-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps/{mobileAppId}/contentVersions/{mobileAppContentId}/files/{mobileAppContentFileId}/renewUpload
```

## <a name="request-headers"></a><span data-ttu-id="f79bc-116">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="f79bc-116">Request headers</span></span>
|<span data-ttu-id="f79bc-117">Заголовок</span><span class="sxs-lookup"><span data-stu-id="f79bc-117">Header</span></span>|<span data-ttu-id="f79bc-118">Значение</span><span class="sxs-lookup"><span data-stu-id="f79bc-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f79bc-119">Авторизация</span><span class="sxs-lookup"><span data-stu-id="f79bc-119">Authorization</span></span>|<span data-ttu-id="f79bc-120">Требуется Bearer &lt;маркер&gt;</span><span class="sxs-lookup"><span data-stu-id="f79bc-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f79bc-121">Принять</span><span class="sxs-lookup"><span data-stu-id="f79bc-121">Accept</span></span>|<span data-ttu-id="f79bc-122">application/json</span><span class="sxs-lookup"><span data-stu-id="f79bc-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f79bc-123">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="f79bc-123">Request body</span></span>
<span data-ttu-id="f79bc-124">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="f79bc-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f79bc-125">Ответ</span><span class="sxs-lookup"><span data-stu-id="f79bc-125">Response</span></span>
<span data-ttu-id="f79bc-126">В случае успешного выполнения это действие возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="f79bc-126">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="f79bc-127">Пример</span><span class="sxs-lookup"><span data-stu-id="f79bc-127">Example</span></span>
### <a name="request"></a><span data-ttu-id="f79bc-128">Запрос</span><span class="sxs-lookup"><span data-stu-id="f79bc-128">Request</span></span>
<span data-ttu-id="f79bc-129">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="f79bc-129">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceAppManagement/mobileApps/{mobileAppId}/contentVersions/{mobileAppContentId}/files/{mobileAppContentFileId}/renewUpload
```

### <a name="response"></a><span data-ttu-id="f79bc-130">Ответ</span><span class="sxs-lookup"><span data-stu-id="f79bc-130">Response</span></span>
<span data-ttu-id="f79bc-p102">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="f79bc-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```








