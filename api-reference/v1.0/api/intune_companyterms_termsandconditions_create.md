# <a name="create-termsandconditions"></a><span data-ttu-id="b5d6b-101">Создание объекта termsAndConditions</span><span class="sxs-lookup"><span data-stu-id="b5d6b-101">Create termsAndConditions</span></span>

> <span data-ttu-id="b5d6b-102">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="b5d6b-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="b5d6b-103">Создание объекта [termsAndConditions](../resources/intune_companyterms_termsandconditions.md).</span><span class="sxs-lookup"><span data-stu-id="b5d6b-103">Create a new [termsAndConditions](../resources/intune_companyterms_termsandconditions.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="b5d6b-104">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="b5d6b-104">Prerequisites</span></span>
<span data-ttu-id="b5d6b-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="b5d6b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="b5d6b-107">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="b5d6b-107">Permission type</span></span>|<span data-ttu-id="b5d6b-108">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="b5d6b-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b5d6b-109">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="b5d6b-109">Delegated (work or school account)</span></span>|<span data-ttu-id="b5d6b-110">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b5d6b-110">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="b5d6b-111">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="b5d6b-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b5d6b-112">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b5d6b-112">Not supported.</span></span>|
|<span data-ttu-id="b5d6b-113">Для приложений</span><span class="sxs-lookup"><span data-stu-id="b5d6b-113">Application</span></span>|<span data-ttu-id="b5d6b-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b5d6b-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="b5d6b-115">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="b5d6b-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/termsAndConditions
```

## <a name="request-headers"></a><span data-ttu-id="b5d6b-116">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="b5d6b-116">Request headers</span></span>
|<span data-ttu-id="b5d6b-117">Заголовок</span><span class="sxs-lookup"><span data-stu-id="b5d6b-117">Header</span></span>|<span data-ttu-id="b5d6b-118">Значение</span><span class="sxs-lookup"><span data-stu-id="b5d6b-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b5d6b-119">Авторизация</span><span class="sxs-lookup"><span data-stu-id="b5d6b-119">Authorization</span></span>|<span data-ttu-id="b5d6b-120">Требуется Bearer &lt;маркер&gt;</span><span class="sxs-lookup"><span data-stu-id="b5d6b-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b5d6b-121">Принять</span><span class="sxs-lookup"><span data-stu-id="b5d6b-121">Accept</span></span>|<span data-ttu-id="b5d6b-122">application/json</span><span class="sxs-lookup"><span data-stu-id="b5d6b-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b5d6b-123">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="b5d6b-123">Request body</span></span>
<span data-ttu-id="b5d6b-124">В тексте запроса добавьте представление объекта termsAndConditions в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="b5d6b-124">In the request body, supply a JSON representation for the termsAndConditions object.</span></span>

<span data-ttu-id="b5d6b-125">В таблице ниже приведены свойства, которые необходимо указывать при создании объекта termsAndConditions.</span><span class="sxs-lookup"><span data-stu-id="b5d6b-125">The following table shows the properties that are required when you create the termsAndConditions.</span></span>

|<span data-ttu-id="b5d6b-126">Свойство</span><span class="sxs-lookup"><span data-stu-id="b5d6b-126">Property</span></span>|<span data-ttu-id="b5d6b-127">Тип</span><span class="sxs-lookup"><span data-stu-id="b5d6b-127">Type</span></span>|<span data-ttu-id="b5d6b-128">Описание</span><span class="sxs-lookup"><span data-stu-id="b5d6b-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b5d6b-129">id</span><span class="sxs-lookup"><span data-stu-id="b5d6b-129">id</span></span>|<span data-ttu-id="b5d6b-130">String</span><span class="sxs-lookup"><span data-stu-id="b5d6b-130">String</span></span>|<span data-ttu-id="b5d6b-131">Уникальный идентификатор политики использования.</span><span class="sxs-lookup"><span data-stu-id="b5d6b-131">Unique identifier of the T&C policy.</span></span>|
|<span data-ttu-id="b5d6b-132">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="b5d6b-132">createdDateTime</span></span>|<span data-ttu-id="b5d6b-133">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b5d6b-133">DateTimeOffset</span></span>|<span data-ttu-id="b5d6b-134">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="b5d6b-134">DateTime the object was created.</span></span>|
|<span data-ttu-id="b5d6b-135">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="b5d6b-135">lastModifiedDateTime</span></span>|<span data-ttu-id="b5d6b-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b5d6b-136">DateTimeOffset</span></span>|<span data-ttu-id="b5d6b-137">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="b5d6b-137">DateTime the object was last modified.</span></span>|
|<span data-ttu-id="b5d6b-138">displayName</span><span class="sxs-lookup"><span data-stu-id="b5d6b-138">displayName</span></span>|<span data-ttu-id="b5d6b-139">String</span><span class="sxs-lookup"><span data-stu-id="b5d6b-139">String</span></span>|<span data-ttu-id="b5d6b-140">Имя политики использования, указанное администратором.</span><span class="sxs-lookup"><span data-stu-id="b5d6b-140">Administrator-supplied name for the T&C policy.</span></span> |
|<span data-ttu-id="b5d6b-141">description</span><span class="sxs-lookup"><span data-stu-id="b5d6b-141">description</span></span>|<span data-ttu-id="b5d6b-142">String</span><span class="sxs-lookup"><span data-stu-id="b5d6b-142">String</span></span>|<span data-ttu-id="b5d6b-143">Описание политики использования, указанное администратором.</span><span class="sxs-lookup"><span data-stu-id="b5d6b-143">Administrator-supplied description of the T&C policy.</span></span>|
|<span data-ttu-id="b5d6b-144">title</span><span class="sxs-lookup"><span data-stu-id="b5d6b-144">title</span></span>|<span data-ttu-id="b5d6b-145">String</span><span class="sxs-lookup"><span data-stu-id="b5d6b-145">String</span></span>|<span data-ttu-id="b5d6b-146">Название условий, указанное администратором.</span><span class="sxs-lookup"><span data-stu-id="b5d6b-146">Administrator-supplied title of the terms and conditions.</span></span> <span data-ttu-id="b5d6b-147">Показывается пользователю при запросе на принятие политики использования.</span><span class="sxs-lookup"><span data-stu-id="b5d6b-147">This is shown to the user on prompts to accept the T&C policy.</span></span>|
|<span data-ttu-id="b5d6b-148">bodyText</span><span class="sxs-lookup"><span data-stu-id="b5d6b-148">bodyText</span></span>|<span data-ttu-id="b5d6b-149">String</span><span class="sxs-lookup"><span data-stu-id="b5d6b-149">String</span></span>|<span data-ttu-id="b5d6b-150">Основной текст условий, заданный администратором (как правило, сами условия).</span><span class="sxs-lookup"><span data-stu-id="b5d6b-150">Administrator-supplied body text of the terms and conditions, typically the terms themselves.</span></span> <span data-ttu-id="b5d6b-151">Показывается пользователю при запросе на принятие политики использования.</span><span class="sxs-lookup"><span data-stu-id="b5d6b-151">This is shown to the user on prompts to accept the T&C policy.</span></span>|
|<span data-ttu-id="b5d6b-152">acceptanceStatement</span><span class="sxs-lookup"><span data-stu-id="b5d6b-152">acceptanceStatement</span></span>|<span data-ttu-id="b5d6b-153">String</span><span class="sxs-lookup"><span data-stu-id="b5d6b-153">String</span></span>|<span data-ttu-id="b5d6b-154">Указанное администратором объяснение условий. Как правило, пользователю объясняется, с чем связано принятие условий, изложенных в соответствующей политике.</span><span class="sxs-lookup"><span data-stu-id="b5d6b-154">Administrator-supplied explanation of the terms and conditions, typically describing what it means to accept the terms and conditions set out in the T&C policy.</span></span> <span data-ttu-id="b5d6b-155">Показывается пользователю при запросе на принятие политики использования.</span><span class="sxs-lookup"><span data-stu-id="b5d6b-155">This is shown to the user on prompts to accept the T&C policy.</span></span>|
|<span data-ttu-id="b5d6b-156">version</span><span class="sxs-lookup"><span data-stu-id="b5d6b-156">version</span></span>|<span data-ttu-id="b5d6b-157">Int32</span><span class="sxs-lookup"><span data-stu-id="b5d6b-157">Int32</span></span>|<span data-ttu-id="b5d6b-158">Целое число, указывающее текущую версию условий.</span><span class="sxs-lookup"><span data-stu-id="b5d6b-158">Integer indicating the current version of the terms.</span></span> <span data-ttu-id="b5d6b-159">Увеличивается, когда администратор вносит изменения в условия и хочет, чтобы пользователи повторно приняли измененную политику.</span><span class="sxs-lookup"><span data-stu-id="b5d6b-159">Incremented when an administrator makes a change to the terms and wishes to require users to re-accept the modified T&C policy.</span></span>|



## <a name="response"></a><span data-ttu-id="b5d6b-160">Отклик</span><span class="sxs-lookup"><span data-stu-id="b5d6b-160">Response</span></span>
<span data-ttu-id="b5d6b-161">В случае успешного выполнения этот метод возвращает код отклика `201 Created` и объект [termsAndConditions](../resources/intune_companyterms_termsandconditions.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="b5d6b-161">If successful, this method returns a `201 Created` response code and a [termsAndConditions](../resources/intune_companyterms_termsandconditions.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b5d6b-162">Пример</span><span class="sxs-lookup"><span data-stu-id="b5d6b-162">Example</span></span>
### <a name="request"></a><span data-ttu-id="b5d6b-163">Запрос</span><span class="sxs-lookup"><span data-stu-id="b5d6b-163">Request</span></span>
<span data-ttu-id="b5d6b-164">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="b5d6b-164">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/termsAndConditions
Content-type: application/json
Content-length: 337

{
  "@odata.type": "#microsoft.graph.termsAndConditions",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "displayName": "Display Name value",
  "description": "Description value",
  "title": "Title value",
  "bodyText": "Body Text value",
  "acceptanceStatement": "Acceptance Statement value",
  "version": 7
}
```

### <a name="response"></a><span data-ttu-id="b5d6b-165">Ответ</span><span class="sxs-lookup"><span data-stu-id="b5d6b-165">Response</span></span>
<span data-ttu-id="b5d6b-p106">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="b5d6b-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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








