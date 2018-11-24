# <a name="delete-deviceandappmanagementroledefinition"></a><span data-ttu-id="3a782-101">Удаление объекта deviceAndAppManagementRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="3a782-101">Delete deviceAndAppManagementRoleDefinition</span></span>

> <span data-ttu-id="3a782-102">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="3a782-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="3a782-103">Удаляет объект [deviceAndAppManagementRoleDefinition](../resources/intune_rbac_deviceandappmanagementroledefinition.md).</span><span class="sxs-lookup"><span data-stu-id="3a782-103">Deletes a [deviceAndAppManagementRoleDefinition](../resources/intune_rbac_deviceandappmanagementroledefinition.md).</span></span>
## <a name="prerequisites"></a><span data-ttu-id="3a782-104">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="3a782-104">Prerequisites</span></span>
<span data-ttu-id="3a782-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="3a782-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="3a782-107">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="3a782-107">Permission type</span></span>|<span data-ttu-id="3a782-108">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="3a782-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3a782-109">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="3a782-109">Delegated (work or school account)</span></span>|<span data-ttu-id="3a782-110">DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3a782-110">DeviceManagementRBAC.ReadWrite.All</span></span>|
|<span data-ttu-id="3a782-111">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="3a782-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3a782-112">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3a782-112">Not supported.</span></span>|
|<span data-ttu-id="3a782-113">Для приложений</span><span class="sxs-lookup"><span data-stu-id="3a782-113">Application</span></span>|<span data-ttu-id="3a782-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3a782-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="3a782-115">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="3a782-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /deviceManagement/roleDefinitions/{roleDefinitionId}
DELETE /deviceManagement/roleDefinitions/{roleDefinitionId}/roleAssignments/{roleAssignmentId}/roleDefinition
```

## <a name="request-headers"></a><span data-ttu-id="3a782-116">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="3a782-116">Request headers</span></span>
|<span data-ttu-id="3a782-117">Заголовок</span><span class="sxs-lookup"><span data-stu-id="3a782-117">Header</span></span>|<span data-ttu-id="3a782-118">Значение</span><span class="sxs-lookup"><span data-stu-id="3a782-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="3a782-119">Авторизация</span><span class="sxs-lookup"><span data-stu-id="3a782-119">Authorization</span></span>|<span data-ttu-id="3a782-120">&lt;Токен&gt; носителя. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="3a782-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="3a782-121">Принять</span><span class="sxs-lookup"><span data-stu-id="3a782-121">Accept</span></span>|<span data-ttu-id="3a782-122">application/json</span><span class="sxs-lookup"><span data-stu-id="3a782-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="3a782-123">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="3a782-123">Request body</span></span>
<span data-ttu-id="3a782-124">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="3a782-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="3a782-125">Отклик</span><span class="sxs-lookup"><span data-stu-id="3a782-125">Response</span></span>
<span data-ttu-id="3a782-126">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="3a782-126">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="3a782-127">Пример</span><span class="sxs-lookup"><span data-stu-id="3a782-127">Example</span></span>
### <a name="request"></a><span data-ttu-id="3a782-128">Запрос</span><span class="sxs-lookup"><span data-stu-id="3a782-128">Request</span></span>
<span data-ttu-id="3a782-129">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="3a782-129">Here is an example of the request.</span></span>
``` http
DELETE https://graph.microsoft.com/v1.0/deviceManagement/roleDefinitions/{roleDefinitionId}
```

### <a name="response"></a><span data-ttu-id="3a782-130">Ответ</span><span class="sxs-lookup"><span data-stu-id="3a782-130">Response</span></span>
<span data-ttu-id="3a782-p102">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="3a782-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```



