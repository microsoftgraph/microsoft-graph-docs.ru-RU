# <a name="update-iosvppebookassignment"></a><span data-ttu-id="8e9f6-101">Обновление объекта iosVppEBookAssignment</span><span class="sxs-lookup"><span data-stu-id="8e9f6-101">Update iosVppEBookAssignment</span></span>

> <span data-ttu-id="8e9f6-102">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="8e9f6-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="8e9f6-103">Обновление свойств объекта [iosVppEBookAssignment](../resources/intune_books_iosvppebookassignment.md).</span><span class="sxs-lookup"><span data-stu-id="8e9f6-103">Update the properties of a [iosVppEBookAssignment](../resources/intune_books_iosvppebookassignment.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="8e9f6-104">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="8e9f6-104">Prerequisites</span></span>
<span data-ttu-id="8e9f6-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="8e9f6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="8e9f6-107">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="8e9f6-107">Permission type</span></span>|<span data-ttu-id="8e9f6-108">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="8e9f6-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8e9f6-109">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="8e9f6-109">Delegated (work or school account)</span></span>|<span data-ttu-id="8e9f6-110">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8e9f6-110">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="8e9f6-111">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="8e9f6-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8e9f6-112">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8e9f6-112">Not supported.</span></span>|
|<span data-ttu-id="8e9f6-113">Для приложений</span><span class="sxs-lookup"><span data-stu-id="8e9f6-113">Application</span></span>|<span data-ttu-id="8e9f6-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8e9f6-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="8e9f6-115">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="8e9f6-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/managedEBooks/{managedEBookId}/assignments/{managedEBookAssignmentId}
```

## <a name="request-headers"></a><span data-ttu-id="8e9f6-116">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="8e9f6-116">Request headers</span></span>
|<span data-ttu-id="8e9f6-117">Заголовок</span><span class="sxs-lookup"><span data-stu-id="8e9f6-117">Header</span></span>|<span data-ttu-id="8e9f6-118">Значение</span><span class="sxs-lookup"><span data-stu-id="8e9f6-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="8e9f6-119">Авторизация</span><span class="sxs-lookup"><span data-stu-id="8e9f6-119">Authorization</span></span>|<span data-ttu-id="8e9f6-120">Требуется Bearer &lt;маркер&gt;</span><span class="sxs-lookup"><span data-stu-id="8e9f6-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="8e9f6-121">Accept</span><span class="sxs-lookup"><span data-stu-id="8e9f6-121">Accept</span></span>|<span data-ttu-id="8e9f6-122">application/json</span><span class="sxs-lookup"><span data-stu-id="8e9f6-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="8e9f6-123">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="8e9f6-123">Request body</span></span>
<span data-ttu-id="8e9f6-124">В тексте запроса добавьте представление объекта [iosVppEBookAssignment](../resources/intune_books_iosvppebookassignment.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="8e9f6-124">In the request body, supply a JSON representation for the [iosVppEBookAssignment](../resources/intune_books_iosvppebookassignment.md) object.</span></span>

<span data-ttu-id="8e9f6-125">В таблице ниже приведены свойства, которые необходимо указывать при создании объекта [iosVppEBookAssignment](../resources/intune_books_iosvppebookassignment.md).</span><span class="sxs-lookup"><span data-stu-id="8e9f6-125">The following table shows the properties that are required when you create the [iosVppEBookAssignment](../resources/intune_books_iosvppebookassignment.md).</span></span>

|<span data-ttu-id="8e9f6-126">Свойство</span><span class="sxs-lookup"><span data-stu-id="8e9f6-126">Property</span></span>|<span data-ttu-id="8e9f6-127">Тип</span><span class="sxs-lookup"><span data-stu-id="8e9f6-127">Type</span></span>|<span data-ttu-id="8e9f6-128">Описание</span><span class="sxs-lookup"><span data-stu-id="8e9f6-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8e9f6-129">ИД</span><span class="sxs-lookup"><span data-stu-id="8e9f6-129">id</span></span>|<span data-ttu-id="8e9f6-130">Строка</span><span class="sxs-lookup"><span data-stu-id="8e9f6-130">String</span></span>|<span data-ttu-id="8e9f6-131">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="8e9f6-131">Key of the entity.</span></span> <span data-ttu-id="8e9f6-132">Наследуется от объекта [managedEBookAssignment](../resources/intune_books_managedebookassignment.md).</span><span class="sxs-lookup"><span data-stu-id="8e9f6-132">Inherited from [managedEBookAssignment](../resources/intune_books_managedebookassignment.md)</span></span>|
|<span data-ttu-id="8e9f6-133">целевой объект</span><span class="sxs-lookup"><span data-stu-id="8e9f6-133">target</span></span>|[<span data-ttu-id="8e9f6-134">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="8e9f6-134">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune_shared_deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="8e9f6-135">Цель назначения электронной книги.</span><span class="sxs-lookup"><span data-stu-id="8e9f6-135">The assignment target for eBook.</span></span> <span data-ttu-id="8e9f6-136">Наследуется от объекта [managedEBookAssignment](../resources/intune_books_managedebookassignment.md).</span><span class="sxs-lookup"><span data-stu-id="8e9f6-136">Inherited from [managedEBookAssignment](../resources/intune_books_managedebookassignment.md)</span></span>|
|<span data-ttu-id="8e9f6-137">installIntent</span><span class="sxs-lookup"><span data-stu-id="8e9f6-137">installIntent</span></span>|[<span data-ttu-id="8e9f6-138">installIntent</span><span class="sxs-lookup"><span data-stu-id="8e9f6-138">installIntent</span></span>](../resources/intune_shared_installintent.md)|<span data-ttu-id="8e9f6-139">Цель установки электронной книги.</span><span class="sxs-lookup"><span data-stu-id="8e9f6-139">The install intent for eBook.</span></span> <span data-ttu-id="8e9f6-140">Унаследовано от [managedEBookAssignment](../resources/intune_books_managedebookassignment.md).</span><span class="sxs-lookup"><span data-stu-id="8e9f6-140">Inherited from [managedEBookAssignment](../resources/intune_books_managedebookassignment.md)</span></span> <span data-ttu-id="8e9f6-141">Возможные значения: `available`, `required`, `uninstall`, `availableWithoutEnrollment`.</span><span class="sxs-lookup"><span data-stu-id="8e9f6-141">The possible values are `available`, `required`, `uninstall`, `availableWithoutEnrollment`, , , , , , , , or .</span></span>|



## <a name="response"></a><span data-ttu-id="8e9f6-142">Ответ</span><span class="sxs-lookup"><span data-stu-id="8e9f6-142">Response</span></span>
<span data-ttu-id="8e9f6-143">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и обновленный объект [iosVppEBookAssignment](../resources/intune_books_iosvppebookassignment.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="8e9f6-143">If successful, this method returns a `200 OK` response code and an updated [iosVppEBookAssignment](../resources/intune_books_iosvppebookassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8e9f6-144">Пример</span><span class="sxs-lookup"><span data-stu-id="8e9f6-144">Example</span></span>
### <a name="request"></a><span data-ttu-id="8e9f6-145">Запрос</span><span class="sxs-lookup"><span data-stu-id="8e9f6-145">Request</span></span>
<span data-ttu-id="8e9f6-146">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="8e9f6-146">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceAppManagement/managedEBooks/{managedEBookId}/assignments/{managedEBookAssignmentId}
Content-type: application/json
Content-length: 133

{
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  },
  "installIntent": "required"
}
```

### <a name="response"></a><span data-ttu-id="8e9f6-147">Ответ</span><span class="sxs-lookup"><span data-stu-id="8e9f6-147">Response</span></span>
<span data-ttu-id="8e9f6-p105">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="8e9f6-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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



