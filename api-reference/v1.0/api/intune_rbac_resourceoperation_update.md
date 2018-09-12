# <a name="update-resourceoperation"></a><span data-ttu-id="4f8fe-101">Обновление объекта resourceOperation</span><span class="sxs-lookup"><span data-stu-id="4f8fe-101">Update resourceOperation</span></span>

> <span data-ttu-id="4f8fe-102">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="4f8fe-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="4f8fe-103">Обновляет свойства объекта [resourceOperation](../resources/intune_rbac_resourceoperation.md).</span><span class="sxs-lookup"><span data-stu-id="4f8fe-103">Update the properties of a [resourceOperation](../resources/intune_rbac_resourceoperation.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="4f8fe-104">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="4f8fe-104">Prerequisites</span></span>
<span data-ttu-id="4f8fe-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="4f8fe-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="4f8fe-107">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="4f8fe-107">Permission type</span></span>|<span data-ttu-id="4f8fe-108">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="4f8fe-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4f8fe-109">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="4f8fe-109">Delegated (work or school account)</span></span>|<span data-ttu-id="4f8fe-110">DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4f8fe-110">DeviceManagementRBAC.ReadWrite.All</span></span>|
|<span data-ttu-id="4f8fe-111">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="4f8fe-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4f8fe-112">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4f8fe-112">Not supported.</span></span>|
|<span data-ttu-id="4f8fe-113">Для приложений</span><span class="sxs-lookup"><span data-stu-id="4f8fe-113">Application</span></span>|<span data-ttu-id="4f8fe-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4f8fe-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="4f8fe-115">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="4f8fe-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/resourceOperations/{resourceOperationId}
```

## <a name="request-headers"></a><span data-ttu-id="4f8fe-116">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="4f8fe-116">Request headers</span></span>
|<span data-ttu-id="4f8fe-117">Заголовок</span><span class="sxs-lookup"><span data-stu-id="4f8fe-117">Header</span></span>|<span data-ttu-id="4f8fe-118">Значение</span><span class="sxs-lookup"><span data-stu-id="4f8fe-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="4f8fe-119">Авторизация</span><span class="sxs-lookup"><span data-stu-id="4f8fe-119">Authorization</span></span>|<span data-ttu-id="4f8fe-120">Требуется Bearer &lt;маркер&gt;</span><span class="sxs-lookup"><span data-stu-id="4f8fe-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="4f8fe-121">Принять</span><span class="sxs-lookup"><span data-stu-id="4f8fe-121">Accept</span></span>|<span data-ttu-id="4f8fe-122">application/json</span><span class="sxs-lookup"><span data-stu-id="4f8fe-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4f8fe-123">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="4f8fe-123">Request body</span></span>
<span data-ttu-id="4f8fe-124">В теле запроса добавьте представление объекта [resourceOperation](../resources/intune_rbac_resourceoperation.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="4f8fe-124">In the request body, supply a JSON representation for the [resourceOperation](../resources/intune_rbac_resourceoperation.md) object.</span></span>

<span data-ttu-id="4f8fe-125">Ниже показаны свойства, которые необходимо указывать при создании объекта [resourceOperation](../resources/intune_rbac_resourceoperation.md).</span><span class="sxs-lookup"><span data-stu-id="4f8fe-125">The following table shows the properties that are required when you create the [resourceOperation](../resources/intune_rbac_resourceoperation.md).</span></span>

|<span data-ttu-id="4f8fe-126">Свойство</span><span class="sxs-lookup"><span data-stu-id="4f8fe-126">Property</span></span>|<span data-ttu-id="4f8fe-127">Тип</span><span class="sxs-lookup"><span data-stu-id="4f8fe-127">Type</span></span>|<span data-ttu-id="4f8fe-128">Описание</span><span class="sxs-lookup"><span data-stu-id="4f8fe-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4f8fe-129">id</span><span class="sxs-lookup"><span data-stu-id="4f8fe-129">id</span></span>|<span data-ttu-id="4f8fe-130">Строка</span><span class="sxs-lookup"><span data-stu-id="4f8fe-130">String</span></span>|<span data-ttu-id="4f8fe-131">Ключ операции с ресурсом.</span><span class="sxs-lookup"><span data-stu-id="4f8fe-131">Key of the Resource Operation.</span></span> <span data-ttu-id="4f8fe-132">Доступен только для чтения и создается автоматически.</span><span class="sxs-lookup"><span data-stu-id="4f8fe-132">Read-only, automatically generated.</span></span>|
|<span data-ttu-id="4f8fe-133">resourceName</span><span class="sxs-lookup"><span data-stu-id="4f8fe-133">resourceName</span></span>|<span data-ttu-id="4f8fe-134">Строка</span><span class="sxs-lookup"><span data-stu-id="4f8fe-134">String</span></span>|<span data-ttu-id="4f8fe-135">Имя ресурса, с которым выполняется эта операция.</span><span class="sxs-lookup"><span data-stu-id="4f8fe-135">Name of the Resource this operation is performed on.</span></span>|
|<span data-ttu-id="4f8fe-136">actionName</span><span class="sxs-lookup"><span data-stu-id="4f8fe-136">actionName</span></span>|<span data-ttu-id="4f8fe-137">Строка</span><span class="sxs-lookup"><span data-stu-id="4f8fe-137">String</span></span>|<span data-ttu-id="4f8fe-138">Тип действия, которое выполнит эта операция.</span><span class="sxs-lookup"><span data-stu-id="4f8fe-138">Type of action this operation is going to perform.</span></span> <span data-ttu-id="4f8fe-139">Свойство actionName должно быть максимально кратким (только несколько слов).</span><span class="sxs-lookup"><span data-stu-id="4f8fe-139">The actionName should be concise and limited to as few words as possible.</span></span>|
|<span data-ttu-id="4f8fe-140">description</span><span class="sxs-lookup"><span data-stu-id="4f8fe-140">description</span></span>|<span data-ttu-id="4f8fe-141">Строка</span><span class="sxs-lookup"><span data-stu-id="4f8fe-141">String</span></span>|<span data-ttu-id="4f8fe-142">Описание операции с ресурсом.</span><span class="sxs-lookup"><span data-stu-id="4f8fe-142">Description of the resource operation.</span></span> <span data-ttu-id="4f8fe-143">Используется в тексте, который отображается над обозначением операции при наведении указателя мыши на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="4f8fe-143">The description is used in mouse-over text for the operation when shown in the Azure Portal.</span></span>|



## <a name="response"></a><span data-ttu-id="4f8fe-144">Отклик</span><span class="sxs-lookup"><span data-stu-id="4f8fe-144">Response</span></span>
<span data-ttu-id="4f8fe-145">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и обновленный объект [resourceOperation](../resources/intune_rbac_resourceoperation.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="4f8fe-145">If successful, this method returns a `200 OK` response code and an updated [resourceOperation](../resources/intune_rbac_resourceoperation.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4f8fe-146">Пример</span><span class="sxs-lookup"><span data-stu-id="4f8fe-146">Example</span></span>
### <a name="request"></a><span data-ttu-id="4f8fe-147">Запрос</span><span class="sxs-lookup"><span data-stu-id="4f8fe-147">Request</span></span>
<span data-ttu-id="4f8fe-148">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="4f8fe-148">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/resourceOperations/{resourceOperationId}
Content-type: application/json
Content-length: 122

{
  "resourceName": "Resource Name value",
  "actionName": "Action Name value",
  "description": "Description value"
}
```

### <a name="response"></a><span data-ttu-id="4f8fe-149">Ответ</span><span class="sxs-lookup"><span data-stu-id="4f8fe-149">Response</span></span>
<span data-ttu-id="4f8fe-p105">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="4f8fe-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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








