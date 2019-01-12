---
title: Создание объекта termsAndConditionsAcceptanceStatus
description: Создание объекта termsAndConditionsAcceptanceStatus.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 35ad3e0aebd675a316e4163ba1eafdea6bc4a309
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27976865"
---
# <a name="create-termsandconditionsacceptancestatus"></a><span data-ttu-id="66e43-103">Создание объекта termsAndConditionsAcceptanceStatus</span><span class="sxs-lookup"><span data-stu-id="66e43-103">Create termsAndConditionsAcceptanceStatus</span></span>

> <span data-ttu-id="66e43-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="66e43-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="66e43-105">Создание объекта [termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md).</span><span class="sxs-lookup"><span data-stu-id="66e43-105">Create a new [termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="66e43-106">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="66e43-106">Prerequisites</span></span>
<span data-ttu-id="66e43-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="66e43-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="66e43-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="66e43-109">Permission type</span></span>|<span data-ttu-id="66e43-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="66e43-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="66e43-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="66e43-111">Delegated (work or school account)</span></span>|<span data-ttu-id="66e43-112">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="66e43-112">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="66e43-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="66e43-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="66e43-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="66e43-114">Not supported.</span></span>|
|<span data-ttu-id="66e43-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="66e43-115">Application</span></span>|<span data-ttu-id="66e43-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="66e43-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="66e43-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="66e43-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/termsAndConditions/{termsAndConditionsId}/acceptanceStatuses
```

## <a name="request-headers"></a><span data-ttu-id="66e43-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="66e43-118">Request headers</span></span>
|<span data-ttu-id="66e43-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="66e43-119">Header</span></span>|<span data-ttu-id="66e43-120">Значение</span><span class="sxs-lookup"><span data-stu-id="66e43-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="66e43-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="66e43-121">Authorization</span></span>|<span data-ttu-id="66e43-122">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="66e43-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="66e43-123">Accept</span><span class="sxs-lookup"><span data-stu-id="66e43-123">Accept</span></span>|<span data-ttu-id="66e43-124">application/json</span><span class="sxs-lookup"><span data-stu-id="66e43-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="66e43-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="66e43-125">Request body</span></span>
<span data-ttu-id="66e43-126">В тексте запроса добавьте представление объекта termsAndConditionsAcceptanceStatus в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="66e43-126">In the request body, supply a JSON representation for the termsAndConditionsAcceptanceStatus object.</span></span>

<span data-ttu-id="66e43-127">В таблице ниже приведены свойства, которые необходимо указывать при создании объекта termsAndConditionsAcceptanceStatus.</span><span class="sxs-lookup"><span data-stu-id="66e43-127">The following table shows the properties that are required when you create the termsAndConditionsAcceptanceStatus.</span></span>

|<span data-ttu-id="66e43-128">Свойство</span><span class="sxs-lookup"><span data-stu-id="66e43-128">Property</span></span>|<span data-ttu-id="66e43-129">Тип</span><span class="sxs-lookup"><span data-stu-id="66e43-129">Type</span></span>|<span data-ttu-id="66e43-130">Описание</span><span class="sxs-lookup"><span data-stu-id="66e43-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="66e43-131">id</span><span class="sxs-lookup"><span data-stu-id="66e43-131">id</span></span>|<span data-ttu-id="66e43-132">String</span><span class="sxs-lookup"><span data-stu-id="66e43-132">String</span></span>|<span data-ttu-id="66e43-133">Уникальный идентификатор объекта.</span><span class="sxs-lookup"><span data-stu-id="66e43-133">Unique identifier of the entity.</span></span>|
|<span data-ttu-id="66e43-134">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="66e43-134">userDisplayName</span></span>|<span data-ttu-id="66e43-135">String</span><span class="sxs-lookup"><span data-stu-id="66e43-135">String</span></span>|<span data-ttu-id="66e43-136">Отображает имя пользователя, чье принятие представлено объектом.</span><span class="sxs-lookup"><span data-stu-id="66e43-136">Display name of the user whose acceptance the entity represents.</span></span>|
|<span data-ttu-id="66e43-137">acceptedVersion</span><span class="sxs-lookup"><span data-stu-id="66e43-137">acceptedVersion</span></span>|<span data-ttu-id="66e43-138">Int32</span><span class="sxs-lookup"><span data-stu-id="66e43-138">Int32</span></span>|<span data-ttu-id="66e43-139">Номер последней версии условий, принятых пользователем.</span><span class="sxs-lookup"><span data-stu-id="66e43-139">Most recent version number of the T&C accepted by the user.</span></span>|
|<span data-ttu-id="66e43-140">acceptedDateTime</span><span class="sxs-lookup"><span data-stu-id="66e43-140">acceptedDateTime</span></span>|<span data-ttu-id="66e43-141">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="66e43-141">DateTimeOffset</span></span>|<span data-ttu-id="66e43-142">Дата и время последнего принятия условий пользователем.</span><span class="sxs-lookup"><span data-stu-id="66e43-142">DateTime when the terms were last accepted by the user.</span></span>|



## <a name="response"></a><span data-ttu-id="66e43-143">Отклик</span><span class="sxs-lookup"><span data-stu-id="66e43-143">Response</span></span>
<span data-ttu-id="66e43-144">В случае успешного выполнения этот метод возвращает код отклика `201 Created` и объект [termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="66e43-144">If successful, this method returns a `201 Created` response code and a [termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="66e43-145">Пример</span><span class="sxs-lookup"><span data-stu-id="66e43-145">Example</span></span>
### <a name="request"></a><span data-ttu-id="66e43-146">Запрос</span><span class="sxs-lookup"><span data-stu-id="66e43-146">Request</span></span>
<span data-ttu-id="66e43-147">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="66e43-147">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/termsAndConditions/{termsAndConditionsId}/acceptanceStatuses
Content-type: application/json
Content-length: 211

{
  "@odata.type": "#microsoft.graph.termsAndConditionsAcceptanceStatus",
  "userDisplayName": "User Display Name value",
  "acceptedVersion": 15,
  "acceptedDateTime": "2016-12-31T23:57:43.6165506-08:00"
}
```

### <a name="response"></a><span data-ttu-id="66e43-148">Ответ</span><span class="sxs-lookup"><span data-stu-id="66e43-148">Response</span></span>
<span data-ttu-id="66e43-p102">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="66e43-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



