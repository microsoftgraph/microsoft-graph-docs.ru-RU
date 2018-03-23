# <a name="create-resourceoperation"></a><span data-ttu-id="9d3a9-101">Создание объекта resourceOperation</span><span class="sxs-lookup"><span data-stu-id="9d3a9-101">Create resourceOperation</span></span>

> <span data-ttu-id="9d3a9-102">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="9d3a9-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="9d3a9-103">Создание объекта [resourceOperation](../resources/intune_rbac_resourceoperation.md).</span><span class="sxs-lookup"><span data-stu-id="9d3a9-103">Create a new [plannerBucket](../resources/intune_rbac_resourceoperation.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="9d3a9-104">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="9d3a9-104">Prerequisites</span></span>
<span data-ttu-id="9d3a9-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="9d3a9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="9d3a9-107">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="9d3a9-107">Permission type</span></span>|<span data-ttu-id="9d3a9-108">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="9d3a9-108">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="9d3a9-109">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="9d3a9-109">Delegated (work or school account)</span></span>|<span data-ttu-id="9d3a9-110">DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9d3a9-110">DeviceManagementRBAC.ReadWrite.All</span></span>|
|<span data-ttu-id="9d3a9-111">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="9d3a9-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9d3a9-112">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9d3a9-112">Not supported.</span></span>|
|<span data-ttu-id="9d3a9-113">Для приложений</span><span class="sxs-lookup"><span data-stu-id="9d3a9-113">Application</span></span>|<span data-ttu-id="9d3a9-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9d3a9-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="9d3a9-115">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="9d3a9-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/resourceOperations
```

## <a name="request-headers"></a><span data-ttu-id="9d3a9-116">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="9d3a9-116">Request headers</span></span>
|<span data-ttu-id="9d3a9-117">Заголовок</span><span class="sxs-lookup"><span data-stu-id="9d3a9-117">Header</span></span>|<span data-ttu-id="9d3a9-118">Значение</span><span class="sxs-lookup"><span data-stu-id="9d3a9-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="9d3a9-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="9d3a9-119">Authorization</span></span>|<span data-ttu-id="9d3a9-120">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="9d3a9-120">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="9d3a9-121">Accept</span><span class="sxs-lookup"><span data-stu-id="9d3a9-121">Accept</span></span>|<span data-ttu-id="9d3a9-122">application/json</span><span class="sxs-lookup"><span data-stu-id="9d3a9-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="9d3a9-123">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="9d3a9-123">Request body</span></span>
<span data-ttu-id="9d3a9-124">В теле запроса добавьте представление объекта resourceOperation в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="9d3a9-124">In the request body, supply a JSON representation of TableRow object.</span></span>

<span data-ttu-id="9d3a9-125">В приведенной ниже таблице указаны свойства, необходимые при создании объекта resourceOperation.</span><span class="sxs-lookup"><span data-stu-id="9d3a9-125">The following table shows the properties that are required when you create a user.</span></span>

|<span data-ttu-id="9d3a9-126">Свойство</span><span class="sxs-lookup"><span data-stu-id="9d3a9-126">Property</span></span>|<span data-ttu-id="9d3a9-127">Тип</span><span class="sxs-lookup"><span data-stu-id="9d3a9-127">Type</span></span>|<span data-ttu-id="9d3a9-128">Описание</span><span class="sxs-lookup"><span data-stu-id="9d3a9-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9d3a9-129">id</span><span class="sxs-lookup"><span data-stu-id="9d3a9-129">id</span></span>|<span data-ttu-id="9d3a9-130">String</span><span class="sxs-lookup"><span data-stu-id="9d3a9-130">String</span></span>|<span data-ttu-id="9d3a9-131">Ключ операции с ресурсом.</span><span class="sxs-lookup"><span data-stu-id="9d3a9-131">Key of the Resource Operation.</span></span> <span data-ttu-id="9d3a9-132">Доступен только для чтения и создается автоматически.</span><span class="sxs-lookup"><span data-stu-id="9d3a9-132">Read-only, automatically generated.</span></span>|
|<span data-ttu-id="9d3a9-133">resourceName</span><span class="sxs-lookup"><span data-stu-id="9d3a9-133">resourceName</span></span>|<span data-ttu-id="9d3a9-134">String</span><span class="sxs-lookup"><span data-stu-id="9d3a9-134">String</span></span>|<span data-ttu-id="9d3a9-135">Имя ресурса, с которым выполняется эта операция.</span><span class="sxs-lookup"><span data-stu-id="9d3a9-135">Name of the Resource this operation is performed on.</span></span>|
|<span data-ttu-id="9d3a9-136">actionName</span><span class="sxs-lookup"><span data-stu-id="9d3a9-136">actionName</span></span>|<span data-ttu-id="9d3a9-137">String</span><span class="sxs-lookup"><span data-stu-id="9d3a9-137">String</span></span>|<span data-ttu-id="9d3a9-138">Тип действия, которое выполнит эта операция.</span><span class="sxs-lookup"><span data-stu-id="9d3a9-138">Type of action this operation is going to perform.</span></span> <span data-ttu-id="9d3a9-139">Свойство actionName должно быть максимально кратким (только несколько слов).</span><span class="sxs-lookup"><span data-stu-id="9d3a9-139">The actionName should be concise and limited to as few words as possible.</span></span>|
|<span data-ttu-id="9d3a9-140">description</span><span class="sxs-lookup"><span data-stu-id="9d3a9-140">description</span></span>|<span data-ttu-id="9d3a9-141">String</span><span class="sxs-lookup"><span data-stu-id="9d3a9-141">String</span></span>|<span data-ttu-id="9d3a9-142">Описание операции с ресурсом.</span><span class="sxs-lookup"><span data-stu-id="9d3a9-142">Description of the resource operation.</span></span> <span data-ttu-id="9d3a9-143">Используется в тексте, который отображается над обозначением операции при наведении указателя мыши на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="9d3a9-143">The description is used in mouse-over text for the operation when shown in the Azure Portal.</span></span>|



## <a name="response"></a><span data-ttu-id="9d3a9-144">Отклик</span><span class="sxs-lookup"><span data-stu-id="9d3a9-144">Response</span></span>
<span data-ttu-id="9d3a9-145">В случае успешного выполнения этот метод возвращает код отклика `201 Created` и объект [resourceOperation](../resources/intune_rbac_resourceoperation.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="9d3a9-145">If successful, this method returns a `201 Created` response code and [plannerBucketTaskBoardTaskFormat](../resources/intune_rbac_resourceoperation.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9d3a9-146">Пример</span><span class="sxs-lookup"><span data-stu-id="9d3a9-146">Example</span></span>
### <a name="request"></a><span data-ttu-id="9d3a9-147">Запрос</span><span class="sxs-lookup"><span data-stu-id="9d3a9-147">Request</span></span>
<span data-ttu-id="9d3a9-148">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="9d3a9-148">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/resourceOperations
Content-type: application/json
Content-length: 178

{
  "@odata.type": "#microsoft.graph.resourceOperation",
  "resourceName": "Resource Name value",
  "actionName": "Action Name value",
  "description": "Description value"
}
```

### <a name="response"></a><span data-ttu-id="9d3a9-149">Ответ</span><span class="sxs-lookup"><span data-stu-id="9d3a9-149">Response</span></span>
<span data-ttu-id="9d3a9-p105">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="9d3a9-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 227

{
  "@odata.type": "#microsoft.graph.resourceOperation",
  "id": "232b8fee-8fee-232b-ee8f-2b23ee8f2b23",
  "resourceName": "Resource Name value",
  "actionName": "Action Name value",
  "description": "Description value"
}
```



