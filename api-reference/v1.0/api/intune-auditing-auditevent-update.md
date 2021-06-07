---
title: Update auditEvent
description: Обновление свойств объекта auditEvent.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: e62c5e7fdf8b10b97938574e11ebd94c9e66789c
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/04/2021
ms.locfileid: "52753487"
---
# <a name="update-auditevent"></a><span data-ttu-id="418cc-103">Update auditEvent</span><span class="sxs-lookup"><span data-stu-id="418cc-103">Update auditEvent</span></span>

<span data-ttu-id="418cc-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="418cc-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="418cc-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="418cc-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="418cc-106">Обновление свойств объекта [auditEvent](../resources/intune-auditing-auditevent.md).</span><span class="sxs-lookup"><span data-stu-id="418cc-106">Update the properties of a [auditEvent](../resources/intune-auditing-auditevent.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="418cc-107">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="418cc-107">Prerequisites</span></span>
<span data-ttu-id="418cc-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="418cc-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="418cc-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="418cc-110">Permission type</span></span>|<span data-ttu-id="418cc-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="418cc-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="418cc-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="418cc-112">Delegated (work or school account)</span></span>|<span data-ttu-id="418cc-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="418cc-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="418cc-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="418cc-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="418cc-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="418cc-115">Not supported.</span></span>|
|<span data-ttu-id="418cc-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="418cc-116">Application</span></span>|<span data-ttu-id="418cc-117">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="418cc-117">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="418cc-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="418cc-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/auditEvents/{auditEventId}
```

## <a name="request-headers"></a><span data-ttu-id="418cc-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="418cc-119">Request headers</span></span>
|<span data-ttu-id="418cc-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="418cc-120">Header</span></span>|<span data-ttu-id="418cc-121">Значение</span><span class="sxs-lookup"><span data-stu-id="418cc-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="418cc-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="418cc-122">Authorization</span></span>|<span data-ttu-id="418cc-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="418cc-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="418cc-124">Accept</span><span class="sxs-lookup"><span data-stu-id="418cc-124">Accept</span></span>|<span data-ttu-id="418cc-125">application/json</span><span class="sxs-lookup"><span data-stu-id="418cc-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="418cc-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="418cc-126">Request body</span></span>
<span data-ttu-id="418cc-127">В теле запроса добавьте представление объекта [auditEvent](../resources/intune-auditing-auditevent.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="418cc-127">In the request body, supply a JSON representation for the [auditEvent](../resources/intune-auditing-auditevent.md) object.</span></span>

<span data-ttu-id="418cc-128">Ниже показаны свойства, которые необходимо указывать при создании объекта [auditEvent](../resources/intune-auditing-auditevent.md).</span><span class="sxs-lookup"><span data-stu-id="418cc-128">The following table shows the properties that are required when you create the [auditEvent](../resources/intune-auditing-auditevent.md).</span></span>

|<span data-ttu-id="418cc-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="418cc-129">Property</span></span>|<span data-ttu-id="418cc-130">Тип</span><span class="sxs-lookup"><span data-stu-id="418cc-130">Type</span></span>|<span data-ttu-id="418cc-131">Описание</span><span class="sxs-lookup"><span data-stu-id="418cc-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="418cc-132">id</span><span class="sxs-lookup"><span data-stu-id="418cc-132">id</span></span>|<span data-ttu-id="418cc-133">String</span><span class="sxs-lookup"><span data-stu-id="418cc-133">String</span></span>|<span data-ttu-id="418cc-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="418cc-134">Key of the entity.</span></span>|
|<span data-ttu-id="418cc-135">displayName</span><span class="sxs-lookup"><span data-stu-id="418cc-135">displayName</span></span>|<span data-ttu-id="418cc-136">String</span><span class="sxs-lookup"><span data-stu-id="418cc-136">String</span></span>|<span data-ttu-id="418cc-137">Отображаемое имя события.</span><span class="sxs-lookup"><span data-stu-id="418cc-137">Event display name.</span></span>|
|<span data-ttu-id="418cc-138">componentName</span><span class="sxs-lookup"><span data-stu-id="418cc-138">componentName</span></span>|<span data-ttu-id="418cc-139">String</span><span class="sxs-lookup"><span data-stu-id="418cc-139">String</span></span>|<span data-ttu-id="418cc-140">Имя компонента.</span><span class="sxs-lookup"><span data-stu-id="418cc-140">Component name.</span></span>|
|<span data-ttu-id="418cc-141">actor</span><span class="sxs-lookup"><span data-stu-id="418cc-141">actor</span></span>|[<span data-ttu-id="418cc-142">auditActor</span><span class="sxs-lookup"><span data-stu-id="418cc-142">auditActor</span></span>](../resources/intune-auditing-auditactor.md)|<span data-ttu-id="418cc-143">Пользователь AAD и приложение, связанные с событием аудита.</span><span class="sxs-lookup"><span data-stu-id="418cc-143">AAD user and application that are associated with the audit event.</span></span>|
|<span data-ttu-id="418cc-144">activity</span><span class="sxs-lookup"><span data-stu-id="418cc-144">activity</span></span>|<span data-ttu-id="418cc-145">String</span><span class="sxs-lookup"><span data-stu-id="418cc-145">String</span></span>|<span data-ttu-id="418cc-146">Понятное имя действия.</span><span class="sxs-lookup"><span data-stu-id="418cc-146">Friendly name of the activity.</span></span>|
|<span data-ttu-id="418cc-147">activityDateTime</span><span class="sxs-lookup"><span data-stu-id="418cc-147">activityDateTime</span></span>|<span data-ttu-id="418cc-148">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="418cc-148">DateTimeOffset</span></span>|<span data-ttu-id="418cc-149">Дата и время выполнения действия (в формате UTC).</span><span class="sxs-lookup"><span data-stu-id="418cc-149">The date time in UTC when the activity was performed.</span></span>|
|<span data-ttu-id="418cc-150">activityType</span><span class="sxs-lookup"><span data-stu-id="418cc-150">activityType</span></span>|<span data-ttu-id="418cc-151">String</span><span class="sxs-lookup"><span data-stu-id="418cc-151">String</span></span>|<span data-ttu-id="418cc-152">Тип выполненного действия.</span><span class="sxs-lookup"><span data-stu-id="418cc-152">The type of activity that was being performed.</span></span>|
|<span data-ttu-id="418cc-153">activityOperationType</span><span class="sxs-lookup"><span data-stu-id="418cc-153">activityOperationType</span></span>|<span data-ttu-id="418cc-154">String</span><span class="sxs-lookup"><span data-stu-id="418cc-154">String</span></span>|<span data-ttu-id="418cc-155">Тип операции HTTP для действия.</span><span class="sxs-lookup"><span data-stu-id="418cc-155">The HTTP operation type of the activity.</span></span>|
|<span data-ttu-id="418cc-156">activityResult</span><span class="sxs-lookup"><span data-stu-id="418cc-156">activityResult</span></span>|<span data-ttu-id="418cc-157">String</span><span class="sxs-lookup"><span data-stu-id="418cc-157">String</span></span>|<span data-ttu-id="418cc-158">Результат действия.</span><span class="sxs-lookup"><span data-stu-id="418cc-158">The result of the activity.</span></span>|
|<span data-ttu-id="418cc-159">correlationId</span><span class="sxs-lookup"><span data-stu-id="418cc-159">correlationId</span></span>|<span data-ttu-id="418cc-160">Guid</span><span class="sxs-lookup"><span data-stu-id="418cc-160">Guid</span></span>|<span data-ttu-id="418cc-161">ИД клиентского запроса, используемый для согласования действий в системе.</span><span class="sxs-lookup"><span data-stu-id="418cc-161">The client request Id that is used to correlate activity within the system.</span></span>|
|<span data-ttu-id="418cc-162">resources</span><span class="sxs-lookup"><span data-stu-id="418cc-162">resources</span></span>|<span data-ttu-id="418cc-163">Коллекция [auditResource](../resources/intune-auditing-auditresource.md)</span><span class="sxs-lookup"><span data-stu-id="418cc-163">[auditResource](../resources/intune-auditing-auditresource.md) collection</span></span>|<span data-ttu-id="418cc-164">Изменяемые ресурсы.</span><span class="sxs-lookup"><span data-stu-id="418cc-164">Resources being modified.</span></span>|
|<span data-ttu-id="418cc-165">category</span><span class="sxs-lookup"><span data-stu-id="418cc-165">category</span></span>|<span data-ttu-id="418cc-166">String</span><span class="sxs-lookup"><span data-stu-id="418cc-166">String</span></span>|<span data-ttu-id="418cc-167">Категория аудита.</span><span class="sxs-lookup"><span data-stu-id="418cc-167">Audit category.</span></span>|



## <a name="response"></a><span data-ttu-id="418cc-168">Ответ</span><span class="sxs-lookup"><span data-stu-id="418cc-168">Response</span></span>
<span data-ttu-id="418cc-169">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и обновленный объект [auditEvent](../resources/intune-auditing-auditevent.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="418cc-169">If successful, this method returns a `200 OK` response code and an updated [auditEvent](../resources/intune-auditing-auditevent.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="418cc-170">Пример</span><span class="sxs-lookup"><span data-stu-id="418cc-170">Example</span></span>

### <a name="request"></a><span data-ttu-id="418cc-171">Запрос</span><span class="sxs-lookup"><span data-stu-id="418cc-171">Request</span></span>
<span data-ttu-id="418cc-172">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="418cc-172">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="418cc-173">Отклик</span><span class="sxs-lookup"><span data-stu-id="418cc-173">Response</span></span>
<span data-ttu-id="418cc-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="418cc-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




