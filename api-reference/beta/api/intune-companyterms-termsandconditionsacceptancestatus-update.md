---
title: Обновление объекта termsAndConditionsAcceptanceStatus
description: Обновление свойств объекта termsAndConditionsAcceptanceStatus.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 548026bf033195364c0bda979f1501e62831ed13
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29420544"
---
# <a name="update-termsandconditionsacceptancestatus"></a><span data-ttu-id="b3e3f-103">Обновление объекта termsAndConditionsAcceptanceStatus</span><span class="sxs-lookup"><span data-stu-id="b3e3f-103">Update termsAndConditionsAcceptanceStatus</span></span>

> <span data-ttu-id="b3e3f-104">**Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="b3e3f-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="b3e3f-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b3e3f-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="b3e3f-106">**Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="b3e3f-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b3e3f-107">Обновление свойств объекта [termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md).</span><span class="sxs-lookup"><span data-stu-id="b3e3f-107">Update the properties of a [termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="b3e3f-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="b3e3f-108">Prerequisites</span></span>
<span data-ttu-id="b3e3f-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="b3e3f-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="b3e3f-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="b3e3f-111">Permission type</span></span>|<span data-ttu-id="b3e3f-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="b3e3f-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b3e3f-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="b3e3f-113">Delegated (work or school account)</span></span>|<span data-ttu-id="b3e3f-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b3e3f-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="b3e3f-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="b3e3f-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b3e3f-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b3e3f-116">Not supported.</span></span>|
|<span data-ttu-id="b3e3f-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="b3e3f-117">Application</span></span>|<span data-ttu-id="b3e3f-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b3e3f-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="b3e3f-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="b3e3f-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/termsAndConditions/{termsAndConditionsId}/acceptanceStatuses/{termsAndConditionsAcceptanceStatusId}
```

## <a name="request-headers"></a><span data-ttu-id="b3e3f-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="b3e3f-120">Request headers</span></span>
|<span data-ttu-id="b3e3f-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="b3e3f-121">Header</span></span>|<span data-ttu-id="b3e3f-122">Значение</span><span class="sxs-lookup"><span data-stu-id="b3e3f-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b3e3f-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="b3e3f-123">Authorization</span></span>|<span data-ttu-id="b3e3f-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="b3e3f-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b3e3f-125">Accept</span><span class="sxs-lookup"><span data-stu-id="b3e3f-125">Accept</span></span>|<span data-ttu-id="b3e3f-126">application/json</span><span class="sxs-lookup"><span data-stu-id="b3e3f-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b3e3f-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="b3e3f-127">Request body</span></span>
<span data-ttu-id="b3e3f-128">В тексте запроса добавьте представление объекта [termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="b3e3f-128">In the request body, supply a JSON representation for the [termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md) object.</span></span>

<span data-ttu-id="b3e3f-129">В таблице ниже приведены свойства, которые необходимо указывать при создании объекта [termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md).</span><span class="sxs-lookup"><span data-stu-id="b3e3f-129">The following table shows the properties that are required when you create the [termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md).</span></span>

|<span data-ttu-id="b3e3f-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="b3e3f-130">Property</span></span>|<span data-ttu-id="b3e3f-131">Тип</span><span class="sxs-lookup"><span data-stu-id="b3e3f-131">Type</span></span>|<span data-ttu-id="b3e3f-132">Описание</span><span class="sxs-lookup"><span data-stu-id="b3e3f-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b3e3f-133">id</span><span class="sxs-lookup"><span data-stu-id="b3e3f-133">id</span></span>|<span data-ttu-id="b3e3f-134">String</span><span class="sxs-lookup"><span data-stu-id="b3e3f-134">String</span></span>|<span data-ttu-id="b3e3f-135">Уникальный идентификатор объекта.</span><span class="sxs-lookup"><span data-stu-id="b3e3f-135">Unique identifier of the entity.</span></span>|
|<span data-ttu-id="b3e3f-136">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="b3e3f-136">userDisplayName</span></span>|<span data-ttu-id="b3e3f-137">String</span><span class="sxs-lookup"><span data-stu-id="b3e3f-137">String</span></span>|<span data-ttu-id="b3e3f-138">Отображает имя пользователя, чье принятие представлено объектом.</span><span class="sxs-lookup"><span data-stu-id="b3e3f-138">Display name of the user whose acceptance the entity represents.</span></span>|
|<span data-ttu-id="b3e3f-139">acceptedVersion</span><span class="sxs-lookup"><span data-stu-id="b3e3f-139">acceptedVersion</span></span>|<span data-ttu-id="b3e3f-140">Int32</span><span class="sxs-lookup"><span data-stu-id="b3e3f-140">Int32</span></span>|<span data-ttu-id="b3e3f-141">Номер последней версии условий, принятых пользователем.</span><span class="sxs-lookup"><span data-stu-id="b3e3f-141">Most recent version number of the T&C accepted by the user.</span></span>|
|<span data-ttu-id="b3e3f-142">acceptedDateTime</span><span class="sxs-lookup"><span data-stu-id="b3e3f-142">acceptedDateTime</span></span>|<span data-ttu-id="b3e3f-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b3e3f-143">DateTimeOffset</span></span>|<span data-ttu-id="b3e3f-144">Дата и время последнего принятия условий пользователем.</span><span class="sxs-lookup"><span data-stu-id="b3e3f-144">DateTime when the terms were last accepted by the user.</span></span>|



## <a name="response"></a><span data-ttu-id="b3e3f-145">Отклик</span><span class="sxs-lookup"><span data-stu-id="b3e3f-145">Response</span></span>
<span data-ttu-id="b3e3f-146">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и обновленный объект [termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="b3e3f-146">If successful, this method returns a `200 OK` response code and an updated [termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b3e3f-147">Пример</span><span class="sxs-lookup"><span data-stu-id="b3e3f-147">Example</span></span>

### <a name="request"></a><span data-ttu-id="b3e3f-148">Запрос</span><span class="sxs-lookup"><span data-stu-id="b3e3f-148">Request</span></span>
<span data-ttu-id="b3e3f-149">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="b3e3f-149">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/termsAndConditions/{termsAndConditionsId}/acceptanceStatuses/{termsAndConditionsAcceptanceStatusId}
Content-type: application/json
Content-length: 211

{
  "@odata.type": "#microsoft.graph.termsAndConditionsAcceptanceStatus",
  "userDisplayName": "User Display Name value",
  "acceptedVersion": 15,
  "acceptedDateTime": "2016-12-31T23:57:43.6165506-08:00"
}
```

### <a name="response"></a><span data-ttu-id="b3e3f-150">Отклик</span><span class="sxs-lookup"><span data-stu-id="b3e3f-150">Response</span></span>
<span data-ttu-id="b3e3f-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="b3e3f-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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




