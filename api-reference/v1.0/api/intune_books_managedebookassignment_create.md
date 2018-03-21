# <a name="create-managedebookassignment"></a><span data-ttu-id="08c31-101">Создание объекта managedEBookAssignment</span><span class="sxs-lookup"><span data-stu-id="08c31-101">Create managedEBookAssignment</span></span>

> <span data-ttu-id="08c31-102">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="08c31-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="08c31-103">Создание объекта [managedEBookAssignment](../resources/intune_books_managedebookassignment.md).</span><span class="sxs-lookup"><span data-stu-id="08c31-103">Create a new [plannerBucket](../resources/intune_books_managedebookassignment.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="08c31-104">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="08c31-104">Prerequisites</span></span>
<span data-ttu-id="08c31-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="08c31-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="08c31-107">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="08c31-107">Permission type</span></span>|<span data-ttu-id="08c31-108">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="08c31-108">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="08c31-109">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="08c31-109">Delegated (work or school account)</span></span>|<span data-ttu-id="08c31-110">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="08c31-110">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="08c31-111">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="08c31-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="08c31-112">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="08c31-112">Not supported.</span></span>|
|<span data-ttu-id="08c31-113">Для приложений</span><span class="sxs-lookup"><span data-stu-id="08c31-113">Application</span></span>|<span data-ttu-id="08c31-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="08c31-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="08c31-115">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="08c31-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/managedEBooks/{managedEBookId}/assignments
```

## <a name="request-headers"></a><span data-ttu-id="08c31-116">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="08c31-116">Request headers</span></span>
|<span data-ttu-id="08c31-117">Заголовок</span><span class="sxs-lookup"><span data-stu-id="08c31-117">Header</span></span>|<span data-ttu-id="08c31-118">Значение</span><span class="sxs-lookup"><span data-stu-id="08c31-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="08c31-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="08c31-119">Authorization</span></span>|<span data-ttu-id="08c31-120">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="08c31-120">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="08c31-121">Accept</span><span class="sxs-lookup"><span data-stu-id="08c31-121">Accept</span></span>|<span data-ttu-id="08c31-122">application/json</span><span class="sxs-lookup"><span data-stu-id="08c31-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="08c31-123">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="08c31-123">Request body</span></span>
<span data-ttu-id="08c31-124">В тексте запроса добавьте представление объекта managedEBookAssignment в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="08c31-124">In the request body, supply a JSON representation of the schemaExtension object.</span></span>

<span data-ttu-id="08c31-125">В таблице ниже приведены свойства, которые необходимо указывать при создании объекта managedEBookAssignment.</span><span class="sxs-lookup"><span data-stu-id="08c31-125">The following table shows the properties that are required when you create a user.</span></span>

|<span data-ttu-id="08c31-126">Свойство</span><span class="sxs-lookup"><span data-stu-id="08c31-126">Property</span></span>|<span data-ttu-id="08c31-127">Тип</span><span class="sxs-lookup"><span data-stu-id="08c31-127">Type</span></span>|<span data-ttu-id="08c31-128">Описание</span><span class="sxs-lookup"><span data-stu-id="08c31-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="08c31-129">id</span><span class="sxs-lookup"><span data-stu-id="08c31-129">id</span></span>|<span data-ttu-id="08c31-130">String</span><span class="sxs-lookup"><span data-stu-id="08c31-130">String</span></span>|<span data-ttu-id="08c31-131">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="08c31-131">Key of the setting.</span></span>|
|<span data-ttu-id="08c31-132">target</span><span class="sxs-lookup"><span data-stu-id="08c31-132">target</span></span>|[<span data-ttu-id="08c31-133">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="08c31-133">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune_books_deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="08c31-134">Цель назначения электронной книги.</span><span class="sxs-lookup"><span data-stu-id="08c31-134">The assignment target for eBook.</span></span>|
|<span data-ttu-id="08c31-135">installIntent</span><span class="sxs-lookup"><span data-stu-id="08c31-135">installIntent</span></span>|<span data-ttu-id="08c31-136">String</span><span class="sxs-lookup"><span data-stu-id="08c31-136">String</span></span>|<span data-ttu-id="08c31-137">Цель установки электронной книги.</span><span class="sxs-lookup"><span data-stu-id="08c31-137">The install intent for eBook.</span></span> <span data-ttu-id="08c31-138">Возможные значения: `available`, `required`, `uninstall`, `availableWithoutEnrollment`.</span><span class="sxs-lookup"><span data-stu-id="08c31-138">Possible values are: `available`, `required`, `uninstall`, `availableWithoutEnrollment`.</span></span>|



## <a name="response"></a><span data-ttu-id="08c31-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="08c31-139">Response</span></span>
<span data-ttu-id="08c31-140">В случае успешного выполнения этот метод возвращает код отклика `201 Created` и объект [managedEBookAssignment](../resources/intune_books_managedebookassignment.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="08c31-140">If successful, this method returns a `201 Created` response code and a [ListItemVersion](../resources/intune_books_managedebookassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="08c31-141">Пример</span><span class="sxs-lookup"><span data-stu-id="08c31-141">Example</span></span>
### <a name="request"></a><span data-ttu-id="08c31-142">Запрос</span><span class="sxs-lookup"><span data-stu-id="08c31-142">Request</span></span>
<span data-ttu-id="08c31-143">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="08c31-143">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceAppManagement/managedEBooks/{managedEBookId}/assignments
Content-type: application/json
Content-length: 194

{
  "@odata.type": "#microsoft.graph.managedEBookAssignment",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  },
  "installIntent": "required"
}
```

### <a name="response"></a><span data-ttu-id="08c31-144">Ответ</span><span class="sxs-lookup"><span data-stu-id="08c31-144">Response</span></span>
<span data-ttu-id="08c31-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="08c31-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 243

{
  "@odata.type": "#microsoft.graph.managedEBookAssignment",
  "id": "ae8b0d27-0d27-ae8b-270d-8bae270d8bae",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  },
  "installIntent": "required"
}
```



