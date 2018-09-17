# <a name="create-iosvppebookassignment"></a><span data-ttu-id="83858-101">Создание объекта iosVppEBookAssignment</span><span class="sxs-lookup"><span data-stu-id="83858-101">Create iosVppEBookAssignment</span></span>

> <span data-ttu-id="83858-102">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="83858-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="83858-103">Создание объекта [iosVppEBookAssignment](../resources/intune_books_iosvppebookassignment.md).</span><span class="sxs-lookup"><span data-stu-id="83858-103">Create a new [iosVppEBookAssignment](../resources/intune_books_iosvppebookassignment.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="83858-104">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="83858-104">Prerequisites</span></span>
<span data-ttu-id="83858-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="83858-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="83858-107">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="83858-107">Permission type</span></span>|<span data-ttu-id="83858-108">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="83858-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="83858-109">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="83858-109">Delegated (work or school account)</span></span>|<span data-ttu-id="83858-110">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="83858-110">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="83858-111">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="83858-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="83858-112">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="83858-112">Not supported.</span></span>|
|<span data-ttu-id="83858-113">Для приложений</span><span class="sxs-lookup"><span data-stu-id="83858-113">Application</span></span>|<span data-ttu-id="83858-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="83858-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="83858-115">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="83858-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/managedEBooks/{managedEBookId}/assignments
```

## <a name="request-headers"></a><span data-ttu-id="83858-116">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="83858-116">Request headers</span></span>
|<span data-ttu-id="83858-117">Заголовок</span><span class="sxs-lookup"><span data-stu-id="83858-117">Header</span></span>|<span data-ttu-id="83858-118">Значение</span><span class="sxs-lookup"><span data-stu-id="83858-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="83858-119">Авторизация</span><span class="sxs-lookup"><span data-stu-id="83858-119">Authorization</span></span>|<span data-ttu-id="83858-120">Требуется Bearer &lt;маркер&gt;</span><span class="sxs-lookup"><span data-stu-id="83858-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="83858-121">Принять</span><span class="sxs-lookup"><span data-stu-id="83858-121">Accept</span></span>|<span data-ttu-id="83858-122">приложение/json</span><span class="sxs-lookup"><span data-stu-id="83858-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="83858-123">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="83858-123">Request body</span></span>
<span data-ttu-id="83858-124">В тексте запроса добавьте представление объекта iosVppEBookAssignment в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="83858-124">In the request body, supply a JSON representation for the iosVppEBookAssignment object.</span></span>

<span data-ttu-id="83858-125">В таблице ниже приведены свойства, которые необходимо указывать при создании объекта iosVppEBookAssignment.</span><span class="sxs-lookup"><span data-stu-id="83858-125">The following table shows the properties that are required when you create the iosVppEBookAssignment.</span></span>

|<span data-ttu-id="83858-126">Свойство</span><span class="sxs-lookup"><span data-stu-id="83858-126">Property</span></span>|<span data-ttu-id="83858-127">Тип</span><span class="sxs-lookup"><span data-stu-id="83858-127">Type</span></span>|<span data-ttu-id="83858-128">Описание</span><span class="sxs-lookup"><span data-stu-id="83858-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="83858-129">ИД</span><span class="sxs-lookup"><span data-stu-id="83858-129">id</span></span>|<span data-ttu-id="83858-130">Строка</span><span class="sxs-lookup"><span data-stu-id="83858-130">String</span></span>|<span data-ttu-id="83858-131">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="83858-131">Key of the entity.</span></span> <span data-ttu-id="83858-132">Наследуется от объекта [managedEBookAssignment](../resources/intune_books_managedebookassignment.md).</span><span class="sxs-lookup"><span data-stu-id="83858-132">Inherited from [managedEBookAssignment](../resources/intune_books_managedebookassignment.md)</span></span>|
|<span data-ttu-id="83858-133">целевой</span><span class="sxs-lookup"><span data-stu-id="83858-133">target</span></span>|[<span data-ttu-id="83858-134">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="83858-134">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune_shared_deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="83858-135">Цель назначения электронной книги.</span><span class="sxs-lookup"><span data-stu-id="83858-135">The assignment target for eBook.</span></span> <span data-ttu-id="83858-136">Наследуется от объекта [managedEBookAssignment](../resources/intune_books_managedebookassignment.md).</span><span class="sxs-lookup"><span data-stu-id="83858-136">Inherited from [managedEBookAssignment](../resources/intune_books_managedebookassignment.md)</span></span>|
|<span data-ttu-id="83858-137">installIntent</span><span class="sxs-lookup"><span data-stu-id="83858-137">installIntent</span></span>|[<span data-ttu-id="83858-138">installIntent</span><span class="sxs-lookup"><span data-stu-id="83858-138">installIntent</span></span>](../resources/intune_shared_installintent.md)|<span data-ttu-id="83858-139">Цель установки электронной книги.</span><span class="sxs-lookup"><span data-stu-id="83858-139">The install intent for eBook.</span></span> <span data-ttu-id="83858-140">Унаследовано от [managedEBookAssignment](../resources/intune_books_managedebookassignment.md).</span><span class="sxs-lookup"><span data-stu-id="83858-140">Inherited from [managedEBookAssignment](../resources/intune_books_managedebookassignment.md)</span></span> <span data-ttu-id="83858-141">Возможные значения: `available`, `required`, `uninstall`, `availableWithoutEnrollment`.</span><span class="sxs-lookup"><span data-stu-id="83858-141">Possible values are: `available`, `required`, `uninstall`, `availableWithoutEnrollment`.</span></span>|



## <a name="response"></a><span data-ttu-id="83858-142">Отклик</span><span class="sxs-lookup"><span data-stu-id="83858-142">Response</span></span>
<span data-ttu-id="83858-143">В случае успешного выполнения этот метод возвращает код отклика `201 Created` и объект [iosVppEBookAssignment](../resources/intune_books_iosvppebookassignment.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="83858-143">If successful, this method returns a `201 Created` response code and a [iosVppEBookAssignment](../resources/intune_books_iosvppebookassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="83858-144">Пример</span><span class="sxs-lookup"><span data-stu-id="83858-144">Example</span></span>
### <a name="request"></a><span data-ttu-id="83858-145">Запрос</span><span class="sxs-lookup"><span data-stu-id="83858-145">Request</span></span>
<span data-ttu-id="83858-146">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="83858-146">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="83858-147">Ответ</span><span class="sxs-lookup"><span data-stu-id="83858-147">Response</span></span>
<span data-ttu-id="83858-p105">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="83858-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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








