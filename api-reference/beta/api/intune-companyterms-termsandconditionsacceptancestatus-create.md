---
title: Создание объекта termsAndConditionsAcceptanceStatus
description: Создание объекта termsAndConditionsAcceptanceStatus.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 6f217076b50699c5a7162d025fecb69cad69e9b1
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27859850"
---
# <a name="create-termsandconditionsacceptancestatus"></a><span data-ttu-id="c5fee-103">Создание объекта termsAndConditionsAcceptanceStatus</span><span class="sxs-lookup"><span data-stu-id="c5fee-103">Create termsAndConditionsAcceptanceStatus</span></span>

> <span data-ttu-id="c5fee-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="c5fee-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="c5fee-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c5fee-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="c5fee-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="c5fee-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="c5fee-107">Создание объекта [termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md).</span><span class="sxs-lookup"><span data-stu-id="c5fee-107">Create a new [termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="c5fee-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="c5fee-108">Prerequisites</span></span>
<span data-ttu-id="c5fee-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c5fee-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c5fee-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c5fee-111">Permission type</span></span>|<span data-ttu-id="c5fee-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="c5fee-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c5fee-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c5fee-113">Delegated (work or school account)</span></span>|<span data-ttu-id="c5fee-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c5fee-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="c5fee-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c5fee-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c5fee-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c5fee-116">Not supported.</span></span>|
|<span data-ttu-id="c5fee-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="c5fee-117">Application</span></span>|<span data-ttu-id="c5fee-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c5fee-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="c5fee-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c5fee-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/termsAndConditions/{termsAndConditionsId}/acceptanceStatuses
```

## <a name="request-headers"></a><span data-ttu-id="c5fee-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="c5fee-120">Request headers</span></span>
|<span data-ttu-id="c5fee-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="c5fee-121">Header</span></span>|<span data-ttu-id="c5fee-122">Значение</span><span class="sxs-lookup"><span data-stu-id="c5fee-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c5fee-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="c5fee-123">Authorization</span></span>|<span data-ttu-id="c5fee-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="c5fee-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c5fee-125">Accept</span><span class="sxs-lookup"><span data-stu-id="c5fee-125">Accept</span></span>|<span data-ttu-id="c5fee-126">application/json</span><span class="sxs-lookup"><span data-stu-id="c5fee-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c5fee-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="c5fee-127">Request body</span></span>
<span data-ttu-id="c5fee-128">В тексте запроса добавьте представление объекта termsAndConditionsAcceptanceStatus в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="c5fee-128">In the request body, supply a JSON representation for the termsAndConditionsAcceptanceStatus object.</span></span>

<span data-ttu-id="c5fee-129">В таблице ниже приведены свойства, которые необходимо указывать при создании объекта termsAndConditionsAcceptanceStatus.</span><span class="sxs-lookup"><span data-stu-id="c5fee-129">The following table shows the properties that are required when you create the termsAndConditionsAcceptanceStatus.</span></span>

|<span data-ttu-id="c5fee-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="c5fee-130">Property</span></span>|<span data-ttu-id="c5fee-131">Тип</span><span class="sxs-lookup"><span data-stu-id="c5fee-131">Type</span></span>|<span data-ttu-id="c5fee-132">Описание</span><span class="sxs-lookup"><span data-stu-id="c5fee-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c5fee-133">id</span><span class="sxs-lookup"><span data-stu-id="c5fee-133">id</span></span>|<span data-ttu-id="c5fee-134">String</span><span class="sxs-lookup"><span data-stu-id="c5fee-134">String</span></span>|<span data-ttu-id="c5fee-135">Уникальный идентификатор объекта.</span><span class="sxs-lookup"><span data-stu-id="c5fee-135">Unique identifier of the entity.</span></span>|
|<span data-ttu-id="c5fee-136">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="c5fee-136">userDisplayName</span></span>|<span data-ttu-id="c5fee-137">String</span><span class="sxs-lookup"><span data-stu-id="c5fee-137">String</span></span>|<span data-ttu-id="c5fee-138">Отображает имя пользователя, чье принятие представлено объектом.</span><span class="sxs-lookup"><span data-stu-id="c5fee-138">Display name of the user whose acceptance the entity represents.</span></span>|
|<span data-ttu-id="c5fee-139">acceptedVersion</span><span class="sxs-lookup"><span data-stu-id="c5fee-139">acceptedVersion</span></span>|<span data-ttu-id="c5fee-140">Int32</span><span class="sxs-lookup"><span data-stu-id="c5fee-140">Int32</span></span>|<span data-ttu-id="c5fee-141">Номер последней версии условий, принятых пользователем.</span><span class="sxs-lookup"><span data-stu-id="c5fee-141">Most recent version number of the T&C accepted by the user.</span></span>|
|<span data-ttu-id="c5fee-142">acceptedDateTime</span><span class="sxs-lookup"><span data-stu-id="c5fee-142">acceptedDateTime</span></span>|<span data-ttu-id="c5fee-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c5fee-143">DateTimeOffset</span></span>|<span data-ttu-id="c5fee-144">Дата и время последнего принятия условий пользователем.</span><span class="sxs-lookup"><span data-stu-id="c5fee-144">DateTime when the terms were last accepted by the user.</span></span>|



## <a name="response"></a><span data-ttu-id="c5fee-145">Отклик</span><span class="sxs-lookup"><span data-stu-id="c5fee-145">Response</span></span>
<span data-ttu-id="c5fee-146">В случае успешного выполнения этот метод возвращает код отклика `201 Created` и объект [termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="c5fee-146">If successful, this method returns a `201 Created` response code and a [termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c5fee-147">Пример</span><span class="sxs-lookup"><span data-stu-id="c5fee-147">Example</span></span>
### <a name="request"></a><span data-ttu-id="c5fee-148">Запрос</span><span class="sxs-lookup"><span data-stu-id="c5fee-148">Request</span></span>
<span data-ttu-id="c5fee-149">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="c5fee-149">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/termsAndConditions/{termsAndConditionsId}/acceptanceStatuses
Content-type: application/json
Content-length: 211

{
  "@odata.type": "#microsoft.graph.termsAndConditionsAcceptanceStatus",
  "userDisplayName": "User Display Name value",
  "acceptedVersion": 15,
  "acceptedDateTime": "2016-12-31T23:57:43.6165506-08:00"
}
```

### <a name="response"></a><span data-ttu-id="c5fee-150">Ответ</span><span class="sxs-lookup"><span data-stu-id="c5fee-150">Response</span></span>
<span data-ttu-id="c5fee-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="c5fee-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 260

{
  "@odata.type": "#microsoft.graph.termsAndConditionsAcceptanceStatus",
  "id": "a045ce1a-ce1a-a045-1ace-45a01ace45a0",
  "userDisplayName": "User Display Name value",
  "acceptedVersion": 15,
  "acceptedDateTime": "2016-12-31T23:57:43.6165506-08:00"
}
```





