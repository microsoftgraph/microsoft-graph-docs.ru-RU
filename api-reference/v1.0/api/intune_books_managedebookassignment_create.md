# <a name="create-managedebookassignment"></a><span data-ttu-id="bfddb-101">Создание объекта managedEBookAssignment</span><span class="sxs-lookup"><span data-stu-id="bfddb-101">Create managedEBookAssignment</span></span>

> <span data-ttu-id="bfddb-102">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="bfddb-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="bfddb-103">Создание объекта [managedEBookAssignment](../resources/intune_books_managedebookassignment.md).</span><span class="sxs-lookup"><span data-stu-id="bfddb-103">Create a new [managedEBookAssignment](../resources/intune_books_managedebookassignment.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="bfddb-104">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="bfddb-104">Prerequisites</span></span>
<span data-ttu-id="bfddb-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="bfddb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="bfddb-107">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="bfddb-107">Permission type</span></span>|<span data-ttu-id="bfddb-108">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="bfddb-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="bfddb-109">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="bfddb-109">Delegated (work or school account)</span></span>|<span data-ttu-id="bfddb-110">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bfddb-110">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="bfddb-111">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="bfddb-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="bfddb-112">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="bfddb-112">Not supported.</span></span>|
|<span data-ttu-id="bfddb-113">Для приложений</span><span class="sxs-lookup"><span data-stu-id="bfddb-113">Application</span></span>|<span data-ttu-id="bfddb-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="bfddb-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="bfddb-115">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="bfddb-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/managedEBooks/{managedEBookId}/assignments
```

## <a name="request-headers"></a><span data-ttu-id="bfddb-116">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="bfddb-116">Request headers</span></span>
|<span data-ttu-id="bfddb-117">Заголовок</span><span class="sxs-lookup"><span data-stu-id="bfddb-117">Header</span></span>|<span data-ttu-id="bfddb-118">Значение</span><span class="sxs-lookup"><span data-stu-id="bfddb-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="bfddb-119">Авторизация</span><span class="sxs-lookup"><span data-stu-id="bfddb-119">Authorization</span></span>|<span data-ttu-id="bfddb-120">Требуется Bearer &lt;маркер&gt;</span><span class="sxs-lookup"><span data-stu-id="bfddb-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="bfddb-121">Accept</span><span class="sxs-lookup"><span data-stu-id="bfddb-121">Accept</span></span>|<span data-ttu-id="bfddb-122">application/json</span><span class="sxs-lookup"><span data-stu-id="bfddb-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="bfddb-123">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="bfddb-123">Request body</span></span>
<span data-ttu-id="bfddb-124">В тексте запроса добавьте представление объекта managedEBookAssignment в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="bfddb-124">In the request body, supply a JSON representation for the managedEBookAssignment object.</span></span>

<span data-ttu-id="bfddb-125">В таблице ниже приведены свойства, которые необходимо указывать при создании объекта managedEBookAssignment.</span><span class="sxs-lookup"><span data-stu-id="bfddb-125">The following table shows the properties that are required when you create the managedEBookAssignment.</span></span>

|<span data-ttu-id="bfddb-126">Свойство</span><span class="sxs-lookup"><span data-stu-id="bfddb-126">Property</span></span>|<span data-ttu-id="bfddb-127">Тип</span><span class="sxs-lookup"><span data-stu-id="bfddb-127">Type</span></span>|<span data-ttu-id="bfddb-128">Описание</span><span class="sxs-lookup"><span data-stu-id="bfddb-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="bfddb-129">id</span><span class="sxs-lookup"><span data-stu-id="bfddb-129">id</span></span>|<span data-ttu-id="bfddb-130">Строка</span><span class="sxs-lookup"><span data-stu-id="bfddb-130">String</span></span>|<span data-ttu-id="bfddb-131">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="bfddb-131">Key of the entity.</span></span>|
|<span data-ttu-id="bfddb-132">target</span><span class="sxs-lookup"><span data-stu-id="bfddb-132">target</span></span>|[<span data-ttu-id="bfddb-133">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="bfddb-133">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune_shared_deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="bfddb-134">Цель назначения электронной книги.</span><span class="sxs-lookup"><span data-stu-id="bfddb-134">The assignment target for eBook.</span></span>|
|<span data-ttu-id="bfddb-135">installIntent</span><span class="sxs-lookup"><span data-stu-id="bfddb-135">installIntent</span></span>|[<span data-ttu-id="bfddb-136">installIntent</span><span class="sxs-lookup"><span data-stu-id="bfddb-136">installIntent</span></span>](../resources/intune_shared_installintent.md)|<span data-ttu-id="bfddb-137">Цель установки электронной книги.</span><span class="sxs-lookup"><span data-stu-id="bfddb-137">The install intent for eBook.</span></span> <span data-ttu-id="bfddb-138">Возможные значения: `available`, `required`, `uninstall`, `availableWithoutEnrollment`.</span><span class="sxs-lookup"><span data-stu-id="bfddb-138">The possible values are `available`, `required`, `uninstall`, `availableWithoutEnrollment`, , , , , , , , or .</span></span>|



## <a name="response"></a><span data-ttu-id="bfddb-139">Ответ</span><span class="sxs-lookup"><span data-stu-id="bfddb-139">Response</span></span>
<span data-ttu-id="bfddb-140">В случае успешного выполнения этот метод возвращает код отклика `201 Created` и объект [managedEBookAssignment](../resources/intune_books_managedebookassignment.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="bfddb-140">If successful, this method returns a `201 Created` response code and a [managedEBookAssignment](../resources/intune_books_managedebookassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="bfddb-141">Пример</span><span class="sxs-lookup"><span data-stu-id="bfddb-141">Example</span></span>
### <a name="request"></a><span data-ttu-id="bfddb-142">Запрос</span><span class="sxs-lookup"><span data-stu-id="bfddb-142">Request</span></span>
<span data-ttu-id="bfddb-143">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="bfddb-143">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="bfddb-144">Ответ</span><span class="sxs-lookup"><span data-stu-id="bfddb-144">Response</span></span>
<span data-ttu-id="bfddb-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="bfddb-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



