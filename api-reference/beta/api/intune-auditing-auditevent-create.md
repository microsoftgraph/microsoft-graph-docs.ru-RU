---
title: Создание объекта auditEvent
description: Создание объекта auditEvent.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 96e5c18caca325cecdbcb0652f40215287cbcb01
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43408791"
---
# <a name="create-auditevent"></a><span data-ttu-id="50b77-103">Создание объекта auditEvent</span><span class="sxs-lookup"><span data-stu-id="50b77-103">Create auditEvent</span></span>

<span data-ttu-id="50b77-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="50b77-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="50b77-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="50b77-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="50b77-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="50b77-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="50b77-107">Создание объекта [auditEvent](../resources/intune-auditing-auditevent.md).</span><span class="sxs-lookup"><span data-stu-id="50b77-107">Create a new [auditEvent](../resources/intune-auditing-auditevent.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="50b77-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="50b77-108">Prerequisites</span></span>
<span data-ttu-id="50b77-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="50b77-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="50b77-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="50b77-111">Permission type</span></span>|<span data-ttu-id="50b77-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="50b77-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="50b77-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="50b77-113">Delegated (work or school account)</span></span>|<span data-ttu-id="50b77-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="50b77-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="50b77-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="50b77-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="50b77-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="50b77-116">Not supported.</span></span>|
|<span data-ttu-id="50b77-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="50b77-117">Application</span></span>|<span data-ttu-id="50b77-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="50b77-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="50b77-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="50b77-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/auditEvents
```

## <a name="request-headers"></a><span data-ttu-id="50b77-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="50b77-120">Request headers</span></span>
|<span data-ttu-id="50b77-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="50b77-121">Header</span></span>|<span data-ttu-id="50b77-122">Значение</span><span class="sxs-lookup"><span data-stu-id="50b77-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="50b77-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="50b77-123">Authorization</span></span>|<span data-ttu-id="50b77-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="50b77-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="50b77-125">Accept</span><span class="sxs-lookup"><span data-stu-id="50b77-125">Accept</span></span>|<span data-ttu-id="50b77-126">application/json</span><span class="sxs-lookup"><span data-stu-id="50b77-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="50b77-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="50b77-127">Request body</span></span>
<span data-ttu-id="50b77-128">В тексте запроса добавьте представление объекта auditEvent в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="50b77-128">In the request body, supply a JSON representation for the auditEvent object.</span></span>

<span data-ttu-id="50b77-129">В таблице ниже приведены свойства, которые необходимо указывать при создании объекта auditEvent.</span><span class="sxs-lookup"><span data-stu-id="50b77-129">The following table shows the properties that are required when you create the auditEvent.</span></span>

|<span data-ttu-id="50b77-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="50b77-130">Property</span></span>|<span data-ttu-id="50b77-131">Тип</span><span class="sxs-lookup"><span data-stu-id="50b77-131">Type</span></span>|<span data-ttu-id="50b77-132">Описание</span><span class="sxs-lookup"><span data-stu-id="50b77-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="50b77-133">id</span><span class="sxs-lookup"><span data-stu-id="50b77-133">id</span></span>|<span data-ttu-id="50b77-134">Строка</span><span class="sxs-lookup"><span data-stu-id="50b77-134">String</span></span>|<span data-ttu-id="50b77-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="50b77-135">Key of the entity.</span></span>|
|<span data-ttu-id="50b77-136">displayName</span><span class="sxs-lookup"><span data-stu-id="50b77-136">displayName</span></span>|<span data-ttu-id="50b77-137">Строка</span><span class="sxs-lookup"><span data-stu-id="50b77-137">String</span></span>|<span data-ttu-id="50b77-138">Отображаемое имя события.</span><span class="sxs-lookup"><span data-stu-id="50b77-138">Event display name.</span></span>|
|<span data-ttu-id="50b77-139">componentName</span><span class="sxs-lookup"><span data-stu-id="50b77-139">componentName</span></span>|<span data-ttu-id="50b77-140">String</span><span class="sxs-lookup"><span data-stu-id="50b77-140">String</span></span>|<span data-ttu-id="50b77-141">Имя компонента.</span><span class="sxs-lookup"><span data-stu-id="50b77-141">Component name.</span></span>|
|<span data-ttu-id="50b77-142">actor</span><span class="sxs-lookup"><span data-stu-id="50b77-142">actor</span></span>|[<span data-ttu-id="50b77-143">auditActor</span><span class="sxs-lookup"><span data-stu-id="50b77-143">auditActor</span></span>](../resources/intune-auditing-auditactor.md)|<span data-ttu-id="50b77-144">Пользователь AAD и приложение, связанные с событием аудита.</span><span class="sxs-lookup"><span data-stu-id="50b77-144">AAD user and application that are associated with the audit event.</span></span>|
|<span data-ttu-id="50b77-145">activity</span><span class="sxs-lookup"><span data-stu-id="50b77-145">activity</span></span>|<span data-ttu-id="50b77-146">String</span><span class="sxs-lookup"><span data-stu-id="50b77-146">String</span></span>|<span data-ttu-id="50b77-147">Понятное имя действия.</span><span class="sxs-lookup"><span data-stu-id="50b77-147">Friendly name of the activity.</span></span>|
|<span data-ttu-id="50b77-148">activityDateTime</span><span class="sxs-lookup"><span data-stu-id="50b77-148">activityDateTime</span></span>|<span data-ttu-id="50b77-149">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="50b77-149">DateTimeOffset</span></span>|<span data-ttu-id="50b77-150">Дата и время выполнения действия (в формате UTC).</span><span class="sxs-lookup"><span data-stu-id="50b77-150">The date time in UTC when the activity was performed.</span></span>|
|<span data-ttu-id="50b77-151">activityType</span><span class="sxs-lookup"><span data-stu-id="50b77-151">activityType</span></span>|<span data-ttu-id="50b77-152">String</span><span class="sxs-lookup"><span data-stu-id="50b77-152">String</span></span>|<span data-ttu-id="50b77-153">Тип выполненного действия.</span><span class="sxs-lookup"><span data-stu-id="50b77-153">The type of activity that was being performed.</span></span>|
|<span data-ttu-id="50b77-154">activityOperationType</span><span class="sxs-lookup"><span data-stu-id="50b77-154">activityOperationType</span></span>|<span data-ttu-id="50b77-155">String</span><span class="sxs-lookup"><span data-stu-id="50b77-155">String</span></span>|<span data-ttu-id="50b77-156">Тип операции HTTP для действия.</span><span class="sxs-lookup"><span data-stu-id="50b77-156">The HTTP operation type of the activity.</span></span>|
|<span data-ttu-id="50b77-157">activityResult</span><span class="sxs-lookup"><span data-stu-id="50b77-157">activityResult</span></span>|<span data-ttu-id="50b77-158">String</span><span class="sxs-lookup"><span data-stu-id="50b77-158">String</span></span>|<span data-ttu-id="50b77-159">Результат действия.</span><span class="sxs-lookup"><span data-stu-id="50b77-159">The result of the activity.</span></span>|
|<span data-ttu-id="50b77-160">correlationId</span><span class="sxs-lookup"><span data-stu-id="50b77-160">correlationId</span></span>|<span data-ttu-id="50b77-161">Guid</span><span class="sxs-lookup"><span data-stu-id="50b77-161">Guid</span></span>|<span data-ttu-id="50b77-162">ИД клиентского запроса, используемый для согласования действий в системе.</span><span class="sxs-lookup"><span data-stu-id="50b77-162">The client request Id that is used to correlate activity within the system.</span></span>|
|<span data-ttu-id="50b77-163">resources</span><span class="sxs-lookup"><span data-stu-id="50b77-163">resources</span></span>|<span data-ttu-id="50b77-164">Коллекция [auditResource](../resources/intune-auditing-auditresource.md)</span><span class="sxs-lookup"><span data-stu-id="50b77-164">[auditResource](../resources/intune-auditing-auditresource.md) collection</span></span>|<span data-ttu-id="50b77-165">Изменяемые ресурсы.</span><span class="sxs-lookup"><span data-stu-id="50b77-165">Resources being modified.</span></span>|
|<span data-ttu-id="50b77-166">category</span><span class="sxs-lookup"><span data-stu-id="50b77-166">category</span></span>|<span data-ttu-id="50b77-167">String</span><span class="sxs-lookup"><span data-stu-id="50b77-167">String</span></span>|<span data-ttu-id="50b77-168">Категория аудита.</span><span class="sxs-lookup"><span data-stu-id="50b77-168">Audit category.</span></span>|



## <a name="response"></a><span data-ttu-id="50b77-169">Отклик</span><span class="sxs-lookup"><span data-stu-id="50b77-169">Response</span></span>
<span data-ttu-id="50b77-170">В случае успешного выполнения этот метод возвращает код отклика `201 Created` и объект [auditEvent](../resources/intune-auditing-auditevent.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="50b77-170">If successful, this method returns a `201 Created` response code and a [auditEvent](../resources/intune-auditing-auditevent.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="50b77-171">Пример</span><span class="sxs-lookup"><span data-stu-id="50b77-171">Example</span></span>

### <a name="request"></a><span data-ttu-id="50b77-172">Запрос</span><span class="sxs-lookup"><span data-stu-id="50b77-172">Request</span></span>
<span data-ttu-id="50b77-173">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="50b77-173">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/auditEvents
Content-type: application/json
Content-length: 1603

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
    "userId": "User Id value",
    "userRoleScopeTags": [
      {
        "@odata.type": "microsoft.graph.roleScopeTagInfo",
        "displayName": "Display Name value",
        "roleScopeTagId": "Role Scope Tag Id value"
      }
    ]
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

### <a name="response"></a><span data-ttu-id="50b77-174">Отклик</span><span class="sxs-lookup"><span data-stu-id="50b77-174">Response</span></span>
<span data-ttu-id="50b77-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="50b77-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1652

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
    "userId": "User Id value",
    "userRoleScopeTags": [
      {
        "@odata.type": "microsoft.graph.roleScopeTagInfo",
        "displayName": "Display Name value",
        "roleScopeTagId": "Role Scope Tag Id value"
      }
    ]
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



