---
title: Создание объекта termsAndConditions
description: Создание объекта termsAndConditions.
author: tfitzmac
ms.openlocfilehash: 1eaa9f8a24082813abb3ffbda2c188a1a4e632b4
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27334414"
---
# <a name="create-termsandconditions"></a><span data-ttu-id="0d953-103">Создание объекта termsAndConditions</span><span class="sxs-lookup"><span data-stu-id="0d953-103">Create termsAndConditions</span></span>

> <span data-ttu-id="0d953-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="0d953-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="0d953-105">Создание объекта [termsAndConditions](../resources/intune-companyterms-termsandconditions.md).</span><span class="sxs-lookup"><span data-stu-id="0d953-105">Create a new [termsAndConditions](../resources/intune-companyterms-termsandconditions.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="0d953-106">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="0d953-106">Prerequisites</span></span>
<span data-ttu-id="0d953-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0d953-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0d953-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="0d953-109">Permission type</span></span>|<span data-ttu-id="0d953-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="0d953-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0d953-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="0d953-111">Delegated (work or school account)</span></span>|<span data-ttu-id="0d953-112">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0d953-112">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="0d953-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="0d953-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0d953-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0d953-114">Not supported.</span></span>|
|<span data-ttu-id="0d953-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="0d953-115">Application</span></span>|<span data-ttu-id="0d953-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0d953-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="0d953-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="0d953-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/termsAndConditions
```

## <a name="request-headers"></a><span data-ttu-id="0d953-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="0d953-118">Request headers</span></span>
|<span data-ttu-id="0d953-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="0d953-119">Header</span></span>|<span data-ttu-id="0d953-120">Значение</span><span class="sxs-lookup"><span data-stu-id="0d953-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="0d953-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="0d953-121">Authorization</span></span>|<span data-ttu-id="0d953-122">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="0d953-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="0d953-123">Accept</span><span class="sxs-lookup"><span data-stu-id="0d953-123">Accept</span></span>|<span data-ttu-id="0d953-124">application/json</span><span class="sxs-lookup"><span data-stu-id="0d953-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="0d953-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="0d953-125">Request body</span></span>
<span data-ttu-id="0d953-126">В тексте запроса добавьте представление объекта termsAndConditions в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="0d953-126">In the request body, supply a JSON representation for the termsAndConditions object.</span></span>

<span data-ttu-id="0d953-127">В таблице ниже приведены свойства, которые необходимо указывать при создании объекта termsAndConditions.</span><span class="sxs-lookup"><span data-stu-id="0d953-127">The following table shows the properties that are required when you create the termsAndConditions.</span></span>

|<span data-ttu-id="0d953-128">Свойство</span><span class="sxs-lookup"><span data-stu-id="0d953-128">Property</span></span>|<span data-ttu-id="0d953-129">Тип</span><span class="sxs-lookup"><span data-stu-id="0d953-129">Type</span></span>|<span data-ttu-id="0d953-130">Описание</span><span class="sxs-lookup"><span data-stu-id="0d953-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0d953-131">id</span><span class="sxs-lookup"><span data-stu-id="0d953-131">id</span></span>|<span data-ttu-id="0d953-132">String</span><span class="sxs-lookup"><span data-stu-id="0d953-132">String</span></span>|<span data-ttu-id="0d953-133">Уникальный идентификатор политики использования.</span><span class="sxs-lookup"><span data-stu-id="0d953-133">Unique identifier of the T&C policy.</span></span>|
|<span data-ttu-id="0d953-134">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="0d953-134">createdDateTime</span></span>|<span data-ttu-id="0d953-135">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0d953-135">DateTimeOffset</span></span>|<span data-ttu-id="0d953-136">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="0d953-136">DateTime the object was created.</span></span>|
|<span data-ttu-id="0d953-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="0d953-137">lastModifiedDateTime</span></span>|<span data-ttu-id="0d953-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0d953-138">DateTimeOffset</span></span>|<span data-ttu-id="0d953-139">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="0d953-139">DateTime the object was last modified.</span></span>|
|<span data-ttu-id="0d953-140">displayName</span><span class="sxs-lookup"><span data-stu-id="0d953-140">displayName</span></span>|<span data-ttu-id="0d953-141">String</span><span class="sxs-lookup"><span data-stu-id="0d953-141">String</span></span>|<span data-ttu-id="0d953-142">Имя политики использования, указанное администратором.</span><span class="sxs-lookup"><span data-stu-id="0d953-142">Administrator-supplied name for the T&C policy.</span></span> |
|<span data-ttu-id="0d953-143">описание</span><span class="sxs-lookup"><span data-stu-id="0d953-143">description</span></span>|<span data-ttu-id="0d953-144">String</span><span class="sxs-lookup"><span data-stu-id="0d953-144">String</span></span>|<span data-ttu-id="0d953-145">Описание политики использования, указанное администратором.</span><span class="sxs-lookup"><span data-stu-id="0d953-145">Administrator-supplied description of the T&C policy.</span></span>|
|<span data-ttu-id="0d953-146">title</span><span class="sxs-lookup"><span data-stu-id="0d953-146">title</span></span>|<span data-ttu-id="0d953-147">String</span><span class="sxs-lookup"><span data-stu-id="0d953-147">String</span></span>|<span data-ttu-id="0d953-148">Название условий, указанное администратором.</span><span class="sxs-lookup"><span data-stu-id="0d953-148">Administrator-supplied title of the terms and conditions.</span></span> <span data-ttu-id="0d953-149">Показывается пользователю при запросе на принятие политики использования.</span><span class="sxs-lookup"><span data-stu-id="0d953-149">This is shown to the user on prompts to accept the T&C policy.</span></span>|
|<span data-ttu-id="0d953-150">bodyText</span><span class="sxs-lookup"><span data-stu-id="0d953-150">bodyText</span></span>|<span data-ttu-id="0d953-151">String</span><span class="sxs-lookup"><span data-stu-id="0d953-151">String</span></span>|<span data-ttu-id="0d953-152">Основной текст условий, заданный администратором (как правило, сами условия).</span><span class="sxs-lookup"><span data-stu-id="0d953-152">Administrator-supplied body text of the terms and conditions, typically the terms themselves.</span></span> <span data-ttu-id="0d953-153">Показывается пользователю при запросе на принятие политики использования.</span><span class="sxs-lookup"><span data-stu-id="0d953-153">This is shown to the user on prompts to accept the T&C policy.</span></span>|
|<span data-ttu-id="0d953-154">acceptanceStatement</span><span class="sxs-lookup"><span data-stu-id="0d953-154">acceptanceStatement</span></span>|<span data-ttu-id="0d953-155">String</span><span class="sxs-lookup"><span data-stu-id="0d953-155">String</span></span>|<span data-ttu-id="0d953-156">Указанное администратором объяснение условий. Как правило, пользователю объясняется, с чем связано принятие условий, изложенных в соответствующей политике.</span><span class="sxs-lookup"><span data-stu-id="0d953-156">Administrator-supplied explanation of the terms and conditions, typically describing what it means to accept the terms and conditions set out in the T&C policy.</span></span> <span data-ttu-id="0d953-157">Показывается пользователю при запросе на принятие политики использования.</span><span class="sxs-lookup"><span data-stu-id="0d953-157">This is shown to the user on prompts to accept the T&C policy.</span></span>|
|<span data-ttu-id="0d953-158">version</span><span class="sxs-lookup"><span data-stu-id="0d953-158">version</span></span>|<span data-ttu-id="0d953-159">Int32</span><span class="sxs-lookup"><span data-stu-id="0d953-159">Int32</span></span>|<span data-ttu-id="0d953-160">Целое число, указывающее текущую версию условий.</span><span class="sxs-lookup"><span data-stu-id="0d953-160">Integer indicating the current version of the terms.</span></span> <span data-ttu-id="0d953-161">Увеличивается, когда администратор вносит изменения в условия и хочет, чтобы пользователи повторно приняли измененную политику.</span><span class="sxs-lookup"><span data-stu-id="0d953-161">Incremented when an administrator makes a change to the terms and wishes to require users to re-accept the modified T&C policy.</span></span>|



## <a name="response"></a><span data-ttu-id="0d953-162">Отклик</span><span class="sxs-lookup"><span data-stu-id="0d953-162">Response</span></span>
<span data-ttu-id="0d953-163">В случае успешного выполнения этот метод возвращает код отклика `201 Created` и объект [termsAndConditions](../resources/intune-companyterms-termsandconditions.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="0d953-163">If successful, this method returns a `201 Created` response code and a [termsAndConditions](../resources/intune-companyterms-termsandconditions.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0d953-164">Пример</span><span class="sxs-lookup"><span data-stu-id="0d953-164">Example</span></span>
### <a name="request"></a><span data-ttu-id="0d953-165">Запрос</span><span class="sxs-lookup"><span data-stu-id="0d953-165">Request</span></span>
<span data-ttu-id="0d953-166">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="0d953-166">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/termsAndConditions
Content-type: application/json
Content-length: 273

{
  "@odata.type": "#microsoft.graph.termsAndConditions",
  "displayName": "Display Name value",
  "description": "Description value",
  "title": "Title value",
  "bodyText": "Body Text value",
  "acceptanceStatement": "Acceptance Statement value",
  "version": 7
}
```

### <a name="response"></a><span data-ttu-id="0d953-167">Ответ</span><span class="sxs-lookup"><span data-stu-id="0d953-167">Response</span></span>
<span data-ttu-id="0d953-p106">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="0d953-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



