# <a name="update-termsandconditions"></a><span data-ttu-id="9006c-101">Update termsAndConditions</span><span class="sxs-lookup"><span data-stu-id="9006c-101">Update termsAndConditions</span></span>

> <span data-ttu-id="9006c-102">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="9006c-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="9006c-103">Обновление свойств объекта [termsAndConditions](../resources/intune_companyterms_termsandconditions.md).</span><span class="sxs-lookup"><span data-stu-id="9006c-103">Update the properties of a [calendar](../resources/intune_companyterms_termsandconditions.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="9006c-104">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="9006c-104">Prerequisites</span></span>
<span data-ttu-id="9006c-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, в том числе о выборе разрешений, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="9006c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="9006c-107">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="9006c-107">Permission type</span></span>|<span data-ttu-id="9006c-108">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="9006c-108">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="9006c-109">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="9006c-109">Delegated (work or school account)</span></span>|<span data-ttu-id="9006c-110">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9006c-110">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="9006c-111">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="9006c-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9006c-112">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9006c-112">Not supported.</span></span>|
|<span data-ttu-id="9006c-113">Для приложений</span><span class="sxs-lookup"><span data-stu-id="9006c-113">Application</span></span>|<span data-ttu-id="9006c-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9006c-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="9006c-115">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="9006c-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/termsAndConditions/{termsAndConditionsId}
PATCH /deviceManagement/termsAndConditions/{termsAndConditionsId}/acceptanceStatuses/{termsAndConditionsAcceptanceStatusId}/termsAndConditions
```

## <a name="request-headers"></a><span data-ttu-id="9006c-116">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="9006c-116">Request headers</span></span>
|<span data-ttu-id="9006c-117">Заголовок</span><span class="sxs-lookup"><span data-stu-id="9006c-117">Header</span></span>|<span data-ttu-id="9006c-118">Значение</span><span class="sxs-lookup"><span data-stu-id="9006c-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="9006c-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="9006c-119">Authorization</span></span>|<span data-ttu-id="9006c-120">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="9006c-120">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="9006c-121">Accept</span><span class="sxs-lookup"><span data-stu-id="9006c-121">Accept</span></span>|<span data-ttu-id="9006c-122">application/json</span><span class="sxs-lookup"><span data-stu-id="9006c-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="9006c-123">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="9006c-123">Request body</span></span>
<span data-ttu-id="9006c-124">В тексте запроса добавьте представление объекта [termsAndConditions](../resources/intune_companyterms_termsandconditions.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="9006c-124">In the request body, supply a JSON representation of the [Contact](../resources/intune_companyterms_termsandconditions.md) object.</span></span>

<span data-ttu-id="9006c-125">В таблице ниже приведены свойства, которые необходимо указывать при создании объекта [termsAndConditions](../resources/intune_companyterms_termsandconditions.md).</span><span class="sxs-lookup"><span data-stu-id="9006c-125">The following table shows the properties that are required when you create a user.</span></span>

|<span data-ttu-id="9006c-126">Свойство</span><span class="sxs-lookup"><span data-stu-id="9006c-126">Property</span></span>|<span data-ttu-id="9006c-127">Тип</span><span class="sxs-lookup"><span data-stu-id="9006c-127">Type</span></span>|<span data-ttu-id="9006c-128">Описание</span><span class="sxs-lookup"><span data-stu-id="9006c-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9006c-129">id</span><span class="sxs-lookup"><span data-stu-id="9006c-129">id</span></span>|<span data-ttu-id="9006c-130">String</span><span class="sxs-lookup"><span data-stu-id="9006c-130">String</span></span>|<span data-ttu-id="9006c-131">Уникальный идентификатор политики использования.</span><span class="sxs-lookup"><span data-stu-id="9006c-131">Unique identifier of the T&C policy.</span></span>|
|<span data-ttu-id="9006c-132">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="9006c-132">createdDateTime</span></span>|<span data-ttu-id="9006c-133">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9006c-133">DateTimeOffset</span></span>|<span data-ttu-id="9006c-134">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="9006c-134">DateTime the object was created.</span></span>|
|<span data-ttu-id="9006c-135">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="9006c-135">lastModifiedDateTime</span></span>|<span data-ttu-id="9006c-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9006c-136">DateTimeOffset</span></span>|<span data-ttu-id="9006c-137">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="9006c-137">DateTime the object was last modified.</span></span>|
|<span data-ttu-id="9006c-138">displayName</span><span class="sxs-lookup"><span data-stu-id="9006c-138">displayName</span></span>|<span data-ttu-id="9006c-139">String</span><span class="sxs-lookup"><span data-stu-id="9006c-139">String</span></span>|<span data-ttu-id="9006c-140">Имя политики использования, указанное администратором.</span><span class="sxs-lookup"><span data-stu-id="9006c-140">Administrator-supplied name for the T&C policy.</span></span> |
|<span data-ttu-id="9006c-141">description</span><span class="sxs-lookup"><span data-stu-id="9006c-141">description</span></span>|<span data-ttu-id="9006c-142">String</span><span class="sxs-lookup"><span data-stu-id="9006c-142">String</span></span>|<span data-ttu-id="9006c-143">Описание политики использования, указанное администратором.</span><span class="sxs-lookup"><span data-stu-id="9006c-143">Administrator-supplied description of the T&C policy.</span></span>|
|<span data-ttu-id="9006c-144">title</span><span class="sxs-lookup"><span data-stu-id="9006c-144">title</span></span>|<span data-ttu-id="9006c-145">String</span><span class="sxs-lookup"><span data-stu-id="9006c-145">String</span></span>|<span data-ttu-id="9006c-146">Название условий, указанное администратором.</span><span class="sxs-lookup"><span data-stu-id="9006c-146">Administrator-supplied title of the terms and conditions.</span></span> <span data-ttu-id="9006c-147">Показывается пользователю при запросе на принятие политики использования.</span><span class="sxs-lookup"><span data-stu-id="9006c-147">This is shown to the user on prompts to accept the T&C policy.</span></span>|
|<span data-ttu-id="9006c-148">bodyText</span><span class="sxs-lookup"><span data-stu-id="9006c-148">BodyText</span></span>|<span data-ttu-id="9006c-149">String</span><span class="sxs-lookup"><span data-stu-id="9006c-149">String</span></span>|<span data-ttu-id="9006c-150">Основной текст условий, заданный администратором (как правило, сами условия).</span><span class="sxs-lookup"><span data-stu-id="9006c-150">Administrator-supplied body text of the terms and conditions, typically the terms themselves.</span></span> <span data-ttu-id="9006c-151">Показывается пользователю при запросе на принятие политики использования.</span><span class="sxs-lookup"><span data-stu-id="9006c-151">This is shown to the user on prompts to accept the T&C policy.</span></span>|
|<span data-ttu-id="9006c-152">acceptanceStatement</span><span class="sxs-lookup"><span data-stu-id="9006c-152">acceptanceStatement</span></span>|<span data-ttu-id="9006c-153">String</span><span class="sxs-lookup"><span data-stu-id="9006c-153">String</span></span>|<span data-ttu-id="9006c-154">Указанное администратором объяснение условий. Как правило, пользователю объясняется, с чем связано принятие условий, изложенных в соответствующей политике.</span><span class="sxs-lookup"><span data-stu-id="9006c-154">Administrator-supplied explanation of the terms and conditions, typically describing what it means to accept the terms and conditions set out in the T&C policy.</span></span> <span data-ttu-id="9006c-155">Показывается пользователю при запросе на принятие политики использования.</span><span class="sxs-lookup"><span data-stu-id="9006c-155">This is shown to the user on prompts to accept the T&C policy.</span></span>|
|<span data-ttu-id="9006c-156">version</span><span class="sxs-lookup"><span data-stu-id="9006c-156">version</span></span>|<span data-ttu-id="9006c-157">Int32</span><span class="sxs-lookup"><span data-stu-id="9006c-157">Int32</span></span>|<span data-ttu-id="9006c-158">Целое число, указывающее текущую версию условий.</span><span class="sxs-lookup"><span data-stu-id="9006c-158">Integer indicating the current version of the terms.</span></span> <span data-ttu-id="9006c-159">Увеличивается, когда администратор вносит изменения в условия и хочет, чтобы пользователи повторно приняли измененную политику.</span><span class="sxs-lookup"><span data-stu-id="9006c-159">Incremented when an administrator makes a change to the terms and wishes to require users to re-accept the modified T&C policy.</span></span>|



## <a name="response"></a><span data-ttu-id="9006c-160">Ответ</span><span class="sxs-lookup"><span data-stu-id="9006c-160">Response</span></span>
<span data-ttu-id="9006c-161">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и обновленный объект [termsAndConditions](../resources/intune_companyterms_termsandconditions.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="9006c-161">If successful, this method returns a `200 OK` response code and an updated [contact](../resources/intune_companyterms_termsandconditions.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9006c-162">Пример</span><span class="sxs-lookup"><span data-stu-id="9006c-162">Example</span></span>
### <a name="request"></a><span data-ttu-id="9006c-163">Запрос</span><span class="sxs-lookup"><span data-stu-id="9006c-163">Request</span></span>
<span data-ttu-id="9006c-164">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="9006c-164">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/termsAndConditions/{termsAndConditionsId}
Content-type: application/json
Content-length: 280

{
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "displayName": "Display Name value",
  "description": "Description value",
  "title": "Title value",
  "bodyText": "Body Text value",
  "acceptanceStatement": "Acceptance Statement value",
  "version": 7
}
```

### <a name="response"></a><span data-ttu-id="9006c-165">Ответ</span><span class="sxs-lookup"><span data-stu-id="9006c-165">Response</span></span>
<span data-ttu-id="9006c-p106">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="9006c-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 445

{
  "@odata.type": "#microsoft.graph.termsAndConditions",
  "id": "eefc80cf-80cf-eefc-cf80-fceecf80fcee",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "displayName": "Display Name value",
  "description": "Description value",
  "title": "Title value",
  "bodyText": "Body Text value",
  "acceptanceStatement": "Acceptance Statement value",
  "version": 7
}
```



