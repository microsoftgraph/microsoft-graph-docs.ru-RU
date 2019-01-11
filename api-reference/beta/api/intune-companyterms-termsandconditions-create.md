---
title: Создание объекта termsAndConditions
description: Создание объекта termsAndConditions.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: bea289d293edd7f7ac68c5a1da1388d89c5687e3
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27824327"
---
# <a name="create-termsandconditions"></a><span data-ttu-id="f9798-103">Создание объекта termsAndConditions</span><span class="sxs-lookup"><span data-stu-id="f9798-103">Create termsAndConditions</span></span>

> <span data-ttu-id="f9798-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="f9798-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="f9798-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f9798-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="f9798-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="f9798-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="f9798-107">Создание объекта [termsAndConditions](../resources/intune-companyterms-termsandconditions.md).</span><span class="sxs-lookup"><span data-stu-id="f9798-107">Create a new [termsAndConditions](../resources/intune-companyterms-termsandconditions.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="f9798-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="f9798-108">Prerequisites</span></span>
<span data-ttu-id="f9798-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f9798-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f9798-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f9798-111">Permission type</span></span>|<span data-ttu-id="f9798-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="f9798-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f9798-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f9798-113">Delegated (work or school account)</span></span>|<span data-ttu-id="f9798-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f9798-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="f9798-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f9798-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f9798-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f9798-116">Not supported.</span></span>|
|<span data-ttu-id="f9798-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="f9798-117">Application</span></span>|<span data-ttu-id="f9798-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f9798-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="f9798-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f9798-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/termsAndConditions
```

## <a name="request-headers"></a><span data-ttu-id="f9798-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="f9798-120">Request headers</span></span>
|<span data-ttu-id="f9798-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="f9798-121">Header</span></span>|<span data-ttu-id="f9798-122">Значение</span><span class="sxs-lookup"><span data-stu-id="f9798-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f9798-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="f9798-123">Authorization</span></span>|<span data-ttu-id="f9798-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="f9798-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f9798-125">Accept</span><span class="sxs-lookup"><span data-stu-id="f9798-125">Accept</span></span>|<span data-ttu-id="f9798-126">application/json</span><span class="sxs-lookup"><span data-stu-id="f9798-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f9798-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="f9798-127">Request body</span></span>
<span data-ttu-id="f9798-128">В тексте запроса добавьте представление объекта termsAndConditions в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="f9798-128">In the request body, supply a JSON representation for the termsAndConditions object.</span></span>

<span data-ttu-id="f9798-129">В таблице ниже приведены свойства, которые необходимо указывать при создании объекта termsAndConditions.</span><span class="sxs-lookup"><span data-stu-id="f9798-129">The following table shows the properties that are required when you create the termsAndConditions.</span></span>

|<span data-ttu-id="f9798-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="f9798-130">Property</span></span>|<span data-ttu-id="f9798-131">Тип</span><span class="sxs-lookup"><span data-stu-id="f9798-131">Type</span></span>|<span data-ttu-id="f9798-132">Описание</span><span class="sxs-lookup"><span data-stu-id="f9798-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f9798-133">id</span><span class="sxs-lookup"><span data-stu-id="f9798-133">id</span></span>|<span data-ttu-id="f9798-134">String</span><span class="sxs-lookup"><span data-stu-id="f9798-134">String</span></span>|<span data-ttu-id="f9798-135">Уникальный идентификатор политики использования.</span><span class="sxs-lookup"><span data-stu-id="f9798-135">Unique identifier of the T&C policy.</span></span>|
|<span data-ttu-id="f9798-136">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="f9798-136">createdDateTime</span></span>|<span data-ttu-id="f9798-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f9798-137">DateTimeOffset</span></span>|<span data-ttu-id="f9798-138">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="f9798-138">DateTime the object was created.</span></span>|
|<span data-ttu-id="f9798-139">modifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="f9798-139">modifiedDateTime</span></span>|<span data-ttu-id="f9798-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f9798-140">DateTimeOffset</span></span>|<span data-ttu-id="f9798-141">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="f9798-141">DateTime the object was last modified.</span></span>|
|<span data-ttu-id="f9798-142">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="f9798-142">lastModifiedDateTime</span></span>|<span data-ttu-id="f9798-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f9798-143">DateTimeOffset</span></span>|<span data-ttu-id="f9798-144">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="f9798-144">DateTime the object was last modified.</span></span>|
|<span data-ttu-id="f9798-145">displayName</span><span class="sxs-lookup"><span data-stu-id="f9798-145">displayName</span></span>|<span data-ttu-id="f9798-146">String</span><span class="sxs-lookup"><span data-stu-id="f9798-146">String</span></span>|<span data-ttu-id="f9798-147">Имя политики использования, указанное администратором.</span><span class="sxs-lookup"><span data-stu-id="f9798-147">Administrator-supplied name for the T&C policy.</span></span> |
|<span data-ttu-id="f9798-148">описание</span><span class="sxs-lookup"><span data-stu-id="f9798-148">description</span></span>|<span data-ttu-id="f9798-149">String</span><span class="sxs-lookup"><span data-stu-id="f9798-149">String</span></span>|<span data-ttu-id="f9798-150">Описание политики использования, указанное администратором.</span><span class="sxs-lookup"><span data-stu-id="f9798-150">Administrator-supplied description of the T&C policy.</span></span>|
|<span data-ttu-id="f9798-151">title</span><span class="sxs-lookup"><span data-stu-id="f9798-151">title</span></span>|<span data-ttu-id="f9798-152">String</span><span class="sxs-lookup"><span data-stu-id="f9798-152">String</span></span>|<span data-ttu-id="f9798-153">Название условий, указанное администратором.</span><span class="sxs-lookup"><span data-stu-id="f9798-153">Administrator-supplied title of the terms and conditions.</span></span> <span data-ttu-id="f9798-154">Показывается пользователю при запросе на принятие политики использования.</span><span class="sxs-lookup"><span data-stu-id="f9798-154">This is shown to the user on prompts to accept the T&C policy.</span></span>|
|<span data-ttu-id="f9798-155">bodyText</span><span class="sxs-lookup"><span data-stu-id="f9798-155">bodyText</span></span>|<span data-ttu-id="f9798-156">String</span><span class="sxs-lookup"><span data-stu-id="f9798-156">String</span></span>|<span data-ttu-id="f9798-157">Основной текст условий, заданный администратором (как правило, сами условия).</span><span class="sxs-lookup"><span data-stu-id="f9798-157">Administrator-supplied body text of the terms and conditions, typically the terms themselves.</span></span> <span data-ttu-id="f9798-158">Показывается пользователю при запросе на принятие политики использования.</span><span class="sxs-lookup"><span data-stu-id="f9798-158">This is shown to the user on prompts to accept the T&C policy.</span></span>|
|<span data-ttu-id="f9798-159">acceptanceStatement</span><span class="sxs-lookup"><span data-stu-id="f9798-159">acceptanceStatement</span></span>|<span data-ttu-id="f9798-160">String</span><span class="sxs-lookup"><span data-stu-id="f9798-160">String</span></span>|<span data-ttu-id="f9798-161">Указанное администратором объяснение условий. Как правило, пользователю объясняется, с чем связано принятие условий, изложенных в соответствующей политике.</span><span class="sxs-lookup"><span data-stu-id="f9798-161">Administrator-supplied explanation of the terms and conditions, typically describing what it means to accept the terms and conditions set out in the T&C policy.</span></span> <span data-ttu-id="f9798-162">Показывается пользователю при запросе на принятие политики использования.</span><span class="sxs-lookup"><span data-stu-id="f9798-162">This is shown to the user on prompts to accept the T&C policy.</span></span>|
|<span data-ttu-id="f9798-163">version</span><span class="sxs-lookup"><span data-stu-id="f9798-163">version</span></span>|<span data-ttu-id="f9798-164">Int32</span><span class="sxs-lookup"><span data-stu-id="f9798-164">Int32</span></span>|<span data-ttu-id="f9798-165">Целое число, указывающее текущую версию условий.</span><span class="sxs-lookup"><span data-stu-id="f9798-165">Integer indicating the current version of the terms.</span></span> <span data-ttu-id="f9798-166">Увеличивается, когда администратор вносит изменения в условия и хочет, чтобы пользователи повторно приняли измененную политику.</span><span class="sxs-lookup"><span data-stu-id="f9798-166">Incremented when an administrator makes a change to the terms and wishes to require users to re-accept the modified T&C policy.</span></span>|



## <a name="response"></a><span data-ttu-id="f9798-167">Отклик</span><span class="sxs-lookup"><span data-stu-id="f9798-167">Response</span></span>
<span data-ttu-id="f9798-168">В случае успешного выполнения этот метод возвращает код отклика `201 Created` и объект [termsAndConditions](../resources/intune-companyterms-termsandconditions.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="f9798-168">If successful, this method returns a `201 Created` response code and a [termsAndConditions](../resources/intune-companyterms-termsandconditions.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f9798-169">Пример</span><span class="sxs-lookup"><span data-stu-id="f9798-169">Example</span></span>
### <a name="request"></a><span data-ttu-id="f9798-170">Запрос</span><span class="sxs-lookup"><span data-stu-id="f9798-170">Request</span></span>
<span data-ttu-id="f9798-171">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="f9798-171">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/termsAndConditions
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

### <a name="response"></a><span data-ttu-id="f9798-172">Ответ</span><span class="sxs-lookup"><span data-stu-id="f9798-172">Response</span></span>
<span data-ttu-id="f9798-p107">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="f9798-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 505

{
  "@odata.type": "#microsoft.graph.termsAndConditions",
  "id": "eefc80cf-80cf-eefc-cf80-fceecf80fcee",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "modifiedDateTime": "2017-01-01T00:00:22.8983556-08:00",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "displayName": "Display Name value",
  "description": "Description value",
  "title": "Title value",
  "bodyText": "Body Text value",
  "acceptanceStatement": "Acceptance Statement value",
  "version": 7
}
```





