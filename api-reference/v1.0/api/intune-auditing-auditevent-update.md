---
title: Update auditEvent
description: Обновление свойств объекта auditEvent.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: e2c0d3aa1e92bd8a255deb40ffd95e3e62289dbf
ms.sourcegitcommit: bd5bb20856d4bffe93b2f77f131664849b602dbb
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/02/2019
ms.locfileid: "37358020"
---
# <a name="update-auditevent"></a><span data-ttu-id="fad94-103">Update auditEvent</span><span class="sxs-lookup"><span data-stu-id="fad94-103">Update auditEvent</span></span>

> <span data-ttu-id="fad94-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="fad94-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="fad94-105">Обновление свойств объекта [auditEvent](../resources/intune-auditing-auditevent.md).</span><span class="sxs-lookup"><span data-stu-id="fad94-105">Update the properties of a [auditEvent](../resources/intune-auditing-auditevent.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="fad94-106">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="fad94-106">Prerequisites</span></span>
<span data-ttu-id="fad94-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="fad94-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fad94-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="fad94-109">Permission type</span></span>|<span data-ttu-id="fad94-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="fad94-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="fad94-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="fad94-111">Delegated (work or school account)</span></span>|<span data-ttu-id="fad94-112">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fad94-112">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="fad94-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="fad94-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="fad94-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fad94-114">Not supported.</span></span>|
|<span data-ttu-id="fad94-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="fad94-115">Application</span></span>|<span data-ttu-id="fad94-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fad94-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="fad94-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="fad94-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/auditEvents/{auditEventId}
```

## <a name="request-headers"></a><span data-ttu-id="fad94-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="fad94-118">Request headers</span></span>
|<span data-ttu-id="fad94-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="fad94-119">Header</span></span>|<span data-ttu-id="fad94-120">Значение</span><span class="sxs-lookup"><span data-stu-id="fad94-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="fad94-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="fad94-121">Authorization</span></span>|<span data-ttu-id="fad94-122">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="fad94-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="fad94-123">Accept</span><span class="sxs-lookup"><span data-stu-id="fad94-123">Accept</span></span>|<span data-ttu-id="fad94-124">application/json</span><span class="sxs-lookup"><span data-stu-id="fad94-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="fad94-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="fad94-125">Request body</span></span>
<span data-ttu-id="fad94-126">В теле запроса добавьте представление объекта [auditEvent](../resources/intune-auditing-auditevent.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="fad94-126">In the request body, supply a JSON representation for the [auditEvent](../resources/intune-auditing-auditevent.md) object.</span></span>

<span data-ttu-id="fad94-127">Ниже показаны свойства, которые необходимо указывать при создании объекта [auditEvent](../resources/intune-auditing-auditevent.md).</span><span class="sxs-lookup"><span data-stu-id="fad94-127">The following table shows the properties that are required when you create the [auditEvent](../resources/intune-auditing-auditevent.md).</span></span>

|<span data-ttu-id="fad94-128">Свойство</span><span class="sxs-lookup"><span data-stu-id="fad94-128">Property</span></span>|<span data-ttu-id="fad94-129">Тип</span><span class="sxs-lookup"><span data-stu-id="fad94-129">Type</span></span>|<span data-ttu-id="fad94-130">Описание</span><span class="sxs-lookup"><span data-stu-id="fad94-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fad94-131">id</span><span class="sxs-lookup"><span data-stu-id="fad94-131">id</span></span>|<span data-ttu-id="fad94-132">Строка</span><span class="sxs-lookup"><span data-stu-id="fad94-132">String</span></span>|<span data-ttu-id="fad94-133">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="fad94-133">Key of the entity.</span></span>|
|<span data-ttu-id="fad94-134">displayName</span><span class="sxs-lookup"><span data-stu-id="fad94-134">displayName</span></span>|<span data-ttu-id="fad94-135">Строка</span><span class="sxs-lookup"><span data-stu-id="fad94-135">String</span></span>|<span data-ttu-id="fad94-136">Отображаемое имя события.</span><span class="sxs-lookup"><span data-stu-id="fad94-136">Event display name.</span></span>|
|<span data-ttu-id="fad94-137">componentName</span><span class="sxs-lookup"><span data-stu-id="fad94-137">componentName</span></span>|<span data-ttu-id="fad94-138">String</span><span class="sxs-lookup"><span data-stu-id="fad94-138">String</span></span>|<span data-ttu-id="fad94-139">Имя компонента.</span><span class="sxs-lookup"><span data-stu-id="fad94-139">Component name.</span></span>|
|<span data-ttu-id="fad94-140">actor</span><span class="sxs-lookup"><span data-stu-id="fad94-140">actor</span></span>|[<span data-ttu-id="fad94-141">auditActor</span><span class="sxs-lookup"><span data-stu-id="fad94-141">auditActor</span></span>](../resources/intune-auditing-auditactor.md)|<span data-ttu-id="fad94-142">Пользователь AAD и приложение, связанные с событием аудита.</span><span class="sxs-lookup"><span data-stu-id="fad94-142">AAD user and application that are associated with the audit event.</span></span>|
|<span data-ttu-id="fad94-143">activity</span><span class="sxs-lookup"><span data-stu-id="fad94-143">activity</span></span>|<span data-ttu-id="fad94-144">String</span><span class="sxs-lookup"><span data-stu-id="fad94-144">String</span></span>|<span data-ttu-id="fad94-145">Понятное имя действия.</span><span class="sxs-lookup"><span data-stu-id="fad94-145">Friendly name of the activity.</span></span>|
|<span data-ttu-id="fad94-146">activityDateTime</span><span class="sxs-lookup"><span data-stu-id="fad94-146">activityDateTime</span></span>|<span data-ttu-id="fad94-147">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="fad94-147">DateTimeOffset</span></span>|<span data-ttu-id="fad94-148">Дата и время выполнения действия (в формате UTC).</span><span class="sxs-lookup"><span data-stu-id="fad94-148">The date time in UTC when the activity was performed.</span></span>|
|<span data-ttu-id="fad94-149">activityType</span><span class="sxs-lookup"><span data-stu-id="fad94-149">activityType</span></span>|<span data-ttu-id="fad94-150">String</span><span class="sxs-lookup"><span data-stu-id="fad94-150">String</span></span>|<span data-ttu-id="fad94-151">Тип выполненного действия.</span><span class="sxs-lookup"><span data-stu-id="fad94-151">The type of activity that was being performed.</span></span>|
|<span data-ttu-id="fad94-152">activityOperationType</span><span class="sxs-lookup"><span data-stu-id="fad94-152">activityOperationType</span></span>|<span data-ttu-id="fad94-153">String</span><span class="sxs-lookup"><span data-stu-id="fad94-153">String</span></span>|<span data-ttu-id="fad94-154">Тип операции HTTP для действия.</span><span class="sxs-lookup"><span data-stu-id="fad94-154">The HTTP operation type of the activity.</span></span>|
|<span data-ttu-id="fad94-155">activityResult</span><span class="sxs-lookup"><span data-stu-id="fad94-155">activityResult</span></span>|<span data-ttu-id="fad94-156">String</span><span class="sxs-lookup"><span data-stu-id="fad94-156">String</span></span>|<span data-ttu-id="fad94-157">Результат действия.</span><span class="sxs-lookup"><span data-stu-id="fad94-157">The result of the activity.</span></span>|
|<span data-ttu-id="fad94-158">correlationId</span><span class="sxs-lookup"><span data-stu-id="fad94-158">correlationId</span></span>|<span data-ttu-id="fad94-159">Guid</span><span class="sxs-lookup"><span data-stu-id="fad94-159">Guid</span></span>|<span data-ttu-id="fad94-160">ИД клиентского запроса, используемый для согласования действий в системе.</span><span class="sxs-lookup"><span data-stu-id="fad94-160">The client request Id that is used to correlate activity within the system.</span></span>|
|<span data-ttu-id="fad94-161">resources</span><span class="sxs-lookup"><span data-stu-id="fad94-161">resources</span></span>|<span data-ttu-id="fad94-162">Коллекция [auditResource](../resources/intune-auditing-auditresource.md)</span><span class="sxs-lookup"><span data-stu-id="fad94-162">[auditResource](../resources/intune-auditing-auditresource.md) collection</span></span>|<span data-ttu-id="fad94-163">Изменяемые ресурсы.</span><span class="sxs-lookup"><span data-stu-id="fad94-163">Resources being modified.</span></span>|
|<span data-ttu-id="fad94-164">category</span><span class="sxs-lookup"><span data-stu-id="fad94-164">category</span></span>|<span data-ttu-id="fad94-165">String</span><span class="sxs-lookup"><span data-stu-id="fad94-165">String</span></span>|<span data-ttu-id="fad94-166">Категория аудита.</span><span class="sxs-lookup"><span data-stu-id="fad94-166">Audit category.</span></span>|



## <a name="response"></a><span data-ttu-id="fad94-167">Ответ</span><span class="sxs-lookup"><span data-stu-id="fad94-167">Response</span></span>
<span data-ttu-id="fad94-168">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и обновленный объект [auditEvent](../resources/intune-auditing-auditevent.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="fad94-168">If successful, this method returns a `200 OK` response code and an updated [auditEvent](../resources/intune-auditing-auditevent.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="fad94-169">Пример</span><span class="sxs-lookup"><span data-stu-id="fad94-169">Example</span></span>

### <a name="request"></a><span data-ttu-id="fad94-170">Запрос</span><span class="sxs-lookup"><span data-stu-id="fad94-170">Request</span></span>
<span data-ttu-id="fad94-171">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="fad94-171">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/auditEvents/{auditEventId}
Content-type: application/json
Content-length: 1390

{
  "@odata.type": "#microsoft.graph.auditEvent",
  "displayName": "Display Name value",
  "componentName": "Component Name value",
  "actor": {
    "@odata.type": "microsoft.graph.auditActor",
    "type": "Type value",
    "userPermissions": [
      "User Permissions value"
    ],
    "applicationId": "Application Id value",
    "applicationDisplayName": "Application Display Name value",
    "userPrincipalName": "User Principal Name value",
    "servicePrincipalName": "Service Principal Name value",
    "ipAddress": "Ip Address value",
    "userId": "User Id value"
  },
  "activity": "Activity value",
  "activityDateTime": "2016-12-31T23:59:51.6363086-08:00",
  "activityType": "Activity Type value",
  "activityOperationType": "Activity Operation Type value",
  "activityResult": "Activity Result value",
  "correlationId": "52effe71-fe71-52ef-71fe-ef5271feef52",
  "resources": [
    {
      "@odata.type": "microsoft.graph.auditResource",
      "displayName": "Display Name value",
      "modifiedProperties": [
        {
          "@odata.type": "microsoft.graph.auditProperty",
          "displayName": "Display Name value",
          "oldValue": "Old Value value",
          "newValue": "New Value value"
        }
      ],
      "type": "Type value",
      "resourceId": "Resource Id value"
    }
  ],
  "category": "Category value"
}
```

### <a name="response"></a><span data-ttu-id="fad94-172">Отклик</span><span class="sxs-lookup"><span data-stu-id="fad94-172">Response</span></span>
<span data-ttu-id="fad94-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="fad94-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1439

{
  "@odata.type": "#microsoft.graph.auditEvent",
  "id": "59653ce8-3ce8-5965-e83c-6559e83c6559",
  "displayName": "Display Name value",
  "componentName": "Component Name value",
  "actor": {
    "@odata.type": "microsoft.graph.auditActor",
    "type": "Type value",
    "userPermissions": [
      "User Permissions value"
    ],
    "applicationId": "Application Id value",
    "applicationDisplayName": "Application Display Name value",
    "userPrincipalName": "User Principal Name value",
    "servicePrincipalName": "Service Principal Name value",
    "ipAddress": "Ip Address value",
    "userId": "User Id value"
  },
  "activity": "Activity value",
  "activityDateTime": "2016-12-31T23:59:51.6363086-08:00",
  "activityType": "Activity Type value",
  "activityOperationType": "Activity Operation Type value",
  "activityResult": "Activity Result value",
  "correlationId": "52effe71-fe71-52ef-71fe-ef5271feef52",
  "resources": [
    {
      "@odata.type": "microsoft.graph.auditResource",
      "displayName": "Display Name value",
      "modifiedProperties": [
        {
          "@odata.type": "microsoft.graph.auditProperty",
          "displayName": "Display Name value",
          "oldValue": "Old Value value",
          "newValue": "New Value value"
        }
      ],
      "type": "Type value",
      "resourceId": "Resource Id value"
    }
  ],
  "category": "Category value"
}
```




