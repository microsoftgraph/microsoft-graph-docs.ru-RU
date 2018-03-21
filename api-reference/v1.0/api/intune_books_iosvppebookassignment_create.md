# <a name="create-iosvppebookassignment"></a><span data-ttu-id="ad89d-101">Создание объекта iosVppEBookAssignment</span><span class="sxs-lookup"><span data-stu-id="ad89d-101">Create iosVppEBookAssignment</span></span>

> <span data-ttu-id="ad89d-102">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="ad89d-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="ad89d-103">Создание объекта [iosVppEBookAssignment](../resources/intune_books_iosvppebookassignment.md).</span><span class="sxs-lookup"><span data-stu-id="ad89d-103">Create a new [plannerBucket](../resources/intune_books_iosvppebookassignment.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="ad89d-104">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="ad89d-104">Prerequisites</span></span>
<span data-ttu-id="ad89d-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="ad89d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="ad89d-107">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ad89d-107">Permission type</span></span>|<span data-ttu-id="ad89d-108">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="ad89d-108">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ad89d-109">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ad89d-109">Delegated (work or school account)</span></span>|<span data-ttu-id="ad89d-110">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ad89d-110">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="ad89d-111">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ad89d-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ad89d-112">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ad89d-112">Not supported.</span></span>|
|<span data-ttu-id="ad89d-113">Для приложений</span><span class="sxs-lookup"><span data-stu-id="ad89d-113">Application</span></span>|<span data-ttu-id="ad89d-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ad89d-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="ad89d-115">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ad89d-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/managedEBooks/{managedEBookId}/assignments
```

## <a name="request-headers"></a><span data-ttu-id="ad89d-116">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="ad89d-116">Request headers</span></span>
|<span data-ttu-id="ad89d-117">Заголовок</span><span class="sxs-lookup"><span data-stu-id="ad89d-117">Header</span></span>|<span data-ttu-id="ad89d-118">Значение</span><span class="sxs-lookup"><span data-stu-id="ad89d-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ad89d-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="ad89d-119">Authorization</span></span>|<span data-ttu-id="ad89d-120">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="ad89d-120">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="ad89d-121">Accept</span><span class="sxs-lookup"><span data-stu-id="ad89d-121">Accept</span></span>|<span data-ttu-id="ad89d-122">application/json</span><span class="sxs-lookup"><span data-stu-id="ad89d-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ad89d-123">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="ad89d-123">Request body</span></span>
<span data-ttu-id="ad89d-124">В тексте запроса добавьте представление объекта iosVppEBookAssignment в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="ad89d-124">In the request body, supply a JSON representation of the schemaExtension object.</span></span>

<span data-ttu-id="ad89d-125">В таблице ниже приведены свойства, которые необходимо указывать при создании объекта iosVppEBookAssignment.</span><span class="sxs-lookup"><span data-stu-id="ad89d-125">The following table shows the properties that are required when you create a user.</span></span>

|<span data-ttu-id="ad89d-126">Свойство</span><span class="sxs-lookup"><span data-stu-id="ad89d-126">Property</span></span>|<span data-ttu-id="ad89d-127">Тип</span><span class="sxs-lookup"><span data-stu-id="ad89d-127">Type</span></span>|<span data-ttu-id="ad89d-128">Описание</span><span class="sxs-lookup"><span data-stu-id="ad89d-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ad89d-129">id</span><span class="sxs-lookup"><span data-stu-id="ad89d-129">id</span></span>|<span data-ttu-id="ad89d-130">String</span><span class="sxs-lookup"><span data-stu-id="ad89d-130">String</span></span>|<span data-ttu-id="ad89d-131">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="ad89d-131">Key of the setting.</span></span> <span data-ttu-id="ad89d-132">Наследуется от объекта [managedEBookAssignment](../resources/intune_books_managedebookassignment.md).</span><span class="sxs-lookup"><span data-stu-id="ad89d-132">Inherited from [managedEBookAssignment](../resources/intune_books_managedebookassignment.md)</span></span>|
|<span data-ttu-id="ad89d-133">target</span><span class="sxs-lookup"><span data-stu-id="ad89d-133">target</span></span>|[<span data-ttu-id="ad89d-134">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="ad89d-134">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune_books_deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="ad89d-135">Цель назначения электронной книги.</span><span class="sxs-lookup"><span data-stu-id="ad89d-135">The assignment target for eBook.</span></span> <span data-ttu-id="ad89d-136">Наследуется от объекта [managedEBookAssignment](../resources/intune_books_managedebookassignment.md).</span><span class="sxs-lookup"><span data-stu-id="ad89d-136">Inherited from [managedEBookAssignment](../resources/intune_books_managedebookassignment.md)</span></span>|
|<span data-ttu-id="ad89d-137">installIntent</span><span class="sxs-lookup"><span data-stu-id="ad89d-137">installIntent</span></span>|<span data-ttu-id="ad89d-138">String</span><span class="sxs-lookup"><span data-stu-id="ad89d-138">String</span></span>|<span data-ttu-id="ad89d-139">Цель установки электронной книги.</span><span class="sxs-lookup"><span data-stu-id="ad89d-139">The install intent for eBook.</span></span> <span data-ttu-id="ad89d-140">Наследуется от объекта [managedEBookAssignment](../resources/intune_books_managedebookassignment.md). Возможные значения: `available`, `required`, `uninstall`, `availableWithoutEnrollment`.</span><span class="sxs-lookup"><span data-stu-id="ad89d-140">Inherited from [managedEBookAssignment](../resources/intune_books_managedebookassignment.md) Possible values are: `available`, `required`, `uninstall`, `availableWithoutEnrollment`.</span></span>|



## <a name="response"></a><span data-ttu-id="ad89d-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="ad89d-141">Response</span></span>
<span data-ttu-id="ad89d-142">В случае успешного выполнения этот метод возвращает код отклика `201 Created` и объект [iosVppEBookAssignment](../resources/intune_books_iosvppebookassignment.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="ad89d-142">If successful, this method returns a `201 Created` response code and a [section](../resources/intune_books_iosvppebookassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ad89d-143">Пример</span><span class="sxs-lookup"><span data-stu-id="ad89d-143">Example</span></span>
### <a name="request"></a><span data-ttu-id="ad89d-144">Запрос</span><span class="sxs-lookup"><span data-stu-id="ad89d-144">Request</span></span>
<span data-ttu-id="ad89d-145">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="ad89d-145">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceAppManagement/managedEBooks/{managedEBookId}/assignments
Content-type: application/json
Content-length: 193

{
  "@odata.type": "#microsoft.graph.iosVppEBookAssignment",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  },
  "installIntent": "required"
}
```

### <a name="response"></a><span data-ttu-id="ad89d-146">Ответ</span><span class="sxs-lookup"><span data-stu-id="ad89d-146">Response</span></span>
<span data-ttu-id="ad89d-p105">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="ad89d-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 242

{
  "@odata.type": "#microsoft.graph.iosVppEBookAssignment",
  "id": "48f05789-5789-48f0-8957-f0488957f048",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  },
  "installIntent": "required"
}
```



