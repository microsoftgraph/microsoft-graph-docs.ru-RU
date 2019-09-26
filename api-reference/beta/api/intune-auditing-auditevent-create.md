---
title: Создание объекта auditEvent
description: Создание объекта auditEvent.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: e76837c935e6f3c88f4946684305844ab3c01589
ms.sourcegitcommit: 86903a4730bbd825eabb7f0a1b2429723cc8b1e6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/26/2019
ms.locfileid: "37171556"
---
# <a name="create-auditevent"></a><span data-ttu-id="d489e-103">Создание объекта auditEvent</span><span class="sxs-lookup"><span data-stu-id="d489e-103">Create auditEvent</span></span>

> <span data-ttu-id="d489e-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d489e-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d489e-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="d489e-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d489e-106">Создание объекта [auditEvent](../resources/intune-auditing-auditevent.md).</span><span class="sxs-lookup"><span data-stu-id="d489e-106">Create a new [auditEvent](../resources/intune-auditing-auditevent.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="d489e-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="d489e-107">Prerequisites</span></span>
<span data-ttu-id="d489e-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d489e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d489e-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d489e-110">Permission type</span></span>|<span data-ttu-id="d489e-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="d489e-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d489e-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d489e-112">Delegated (work or school account)</span></span>|<span data-ttu-id="d489e-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d489e-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="d489e-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d489e-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d489e-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d489e-115">Not supported.</span></span>|
|<span data-ttu-id="d489e-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="d489e-116">Application</span></span>|<span data-ttu-id="d489e-117">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d489e-117">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="d489e-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d489e-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/auditEvents
```

## <a name="request-headers"></a><span data-ttu-id="d489e-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="d489e-119">Request headers</span></span>
|<span data-ttu-id="d489e-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="d489e-120">Header</span></span>|<span data-ttu-id="d489e-121">Значение</span><span class="sxs-lookup"><span data-stu-id="d489e-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d489e-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="d489e-122">Authorization</span></span>|<span data-ttu-id="d489e-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="d489e-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d489e-124">Accept</span><span class="sxs-lookup"><span data-stu-id="d489e-124">Accept</span></span>|<span data-ttu-id="d489e-125">application/json</span><span class="sxs-lookup"><span data-stu-id="d489e-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d489e-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="d489e-126">Request body</span></span>
<span data-ttu-id="d489e-127">В тексте запроса добавьте представление объекта auditEvent в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="d489e-127">In the request body, supply a JSON representation for the auditEvent object.</span></span>

<span data-ttu-id="d489e-128">В таблице ниже приведены свойства, которые необходимо указывать при создании объекта auditEvent.</span><span class="sxs-lookup"><span data-stu-id="d489e-128">The following table shows the properties that are required when you create the auditEvent.</span></span>

|<span data-ttu-id="d489e-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="d489e-129">Property</span></span>|<span data-ttu-id="d489e-130">Тип</span><span class="sxs-lookup"><span data-stu-id="d489e-130">Type</span></span>|<span data-ttu-id="d489e-131">Описание</span><span class="sxs-lookup"><span data-stu-id="d489e-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d489e-132">id</span><span class="sxs-lookup"><span data-stu-id="d489e-132">id</span></span>|<span data-ttu-id="d489e-133">Строка</span><span class="sxs-lookup"><span data-stu-id="d489e-133">String</span></span>|<span data-ttu-id="d489e-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="d489e-134">Key of the entity.</span></span>|
|<span data-ttu-id="d489e-135">displayName</span><span class="sxs-lookup"><span data-stu-id="d489e-135">displayName</span></span>|<span data-ttu-id="d489e-136">Строка</span><span class="sxs-lookup"><span data-stu-id="d489e-136">String</span></span>|<span data-ttu-id="d489e-137">Отображаемое имя события.</span><span class="sxs-lookup"><span data-stu-id="d489e-137">Event display name.</span></span>|
|<span data-ttu-id="d489e-138">componentName</span><span class="sxs-lookup"><span data-stu-id="d489e-138">componentName</span></span>|<span data-ttu-id="d489e-139">String.</span><span class="sxs-lookup"><span data-stu-id="d489e-139">String</span></span>|<span data-ttu-id="d489e-140">Имя компонента.</span><span class="sxs-lookup"><span data-stu-id="d489e-140">Component name.</span></span>|
|<span data-ttu-id="d489e-141">actor</span><span class="sxs-lookup"><span data-stu-id="d489e-141">actor</span></span>|[<span data-ttu-id="d489e-142">auditActor</span><span class="sxs-lookup"><span data-stu-id="d489e-142">auditActor</span></span>](../resources/intune-auditing-auditactor.md)|<span data-ttu-id="d489e-143">Пользователь AAD и приложение, связанные с событием аудита.</span><span class="sxs-lookup"><span data-stu-id="d489e-143">AAD user and application that are associated with the audit event.</span></span>|
|<span data-ttu-id="d489e-144">activity</span><span class="sxs-lookup"><span data-stu-id="d489e-144">activity</span></span>|<span data-ttu-id="d489e-145">String.</span><span class="sxs-lookup"><span data-stu-id="d489e-145">String</span></span>|<span data-ttu-id="d489e-146">Понятное имя действия.</span><span class="sxs-lookup"><span data-stu-id="d489e-146">Friendly name of the activity.</span></span>|
|<span data-ttu-id="d489e-147">activityDateTime</span><span class="sxs-lookup"><span data-stu-id="d489e-147">activityDateTime</span></span>|<span data-ttu-id="d489e-148">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d489e-148">DateTimeOffset</span></span>|<span data-ttu-id="d489e-149">Дата и время выполнения действия (в формате UTC).</span><span class="sxs-lookup"><span data-stu-id="d489e-149">The date time in UTC when the activity was performed.</span></span>|
|<span data-ttu-id="d489e-150">activityType</span><span class="sxs-lookup"><span data-stu-id="d489e-150">activityType</span></span>|<span data-ttu-id="d489e-151">String.</span><span class="sxs-lookup"><span data-stu-id="d489e-151">String</span></span>|<span data-ttu-id="d489e-152">Тип выполненного действия.</span><span class="sxs-lookup"><span data-stu-id="d489e-152">The type of activity that was being performed.</span></span>|
|<span data-ttu-id="d489e-153">activityOperationType</span><span class="sxs-lookup"><span data-stu-id="d489e-153">activityOperationType</span></span>|<span data-ttu-id="d489e-154">String.</span><span class="sxs-lookup"><span data-stu-id="d489e-154">String</span></span>|<span data-ttu-id="d489e-155">Тип операции HTTP для действия.</span><span class="sxs-lookup"><span data-stu-id="d489e-155">The HTTP operation type of the activity.</span></span>|
|<span data-ttu-id="d489e-156">activityResult</span><span class="sxs-lookup"><span data-stu-id="d489e-156">activityResult</span></span>|<span data-ttu-id="d489e-157">String</span><span class="sxs-lookup"><span data-stu-id="d489e-157">String</span></span>|<span data-ttu-id="d489e-158">Результат действия.</span><span class="sxs-lookup"><span data-stu-id="d489e-158">The result of the activity.</span></span>|
|<span data-ttu-id="d489e-159">correlationId</span><span class="sxs-lookup"><span data-stu-id="d489e-159">correlationId</span></span>|<span data-ttu-id="d489e-160">Guid</span><span class="sxs-lookup"><span data-stu-id="d489e-160">Guid</span></span>|<span data-ttu-id="d489e-161">ИД клиентского запроса, используемый для согласования действий в системе.</span><span class="sxs-lookup"><span data-stu-id="d489e-161">The client request Id that is used to correlate activity within the system.</span></span>|
|<span data-ttu-id="d489e-162">resources</span><span class="sxs-lookup"><span data-stu-id="d489e-162">resources</span></span>|<span data-ttu-id="d489e-163">Коллекция [auditResource](../resources/intune-auditing-auditresource.md)</span><span class="sxs-lookup"><span data-stu-id="d489e-163">[auditResource](../resources/intune-auditing-auditresource.md) collection</span></span>|<span data-ttu-id="d489e-164">Изменяемые ресурсы.</span><span class="sxs-lookup"><span data-stu-id="d489e-164">Resources being modified.</span></span>|
|<span data-ttu-id="d489e-165">category</span><span class="sxs-lookup"><span data-stu-id="d489e-165">category</span></span>|<span data-ttu-id="d489e-166">String</span><span class="sxs-lookup"><span data-stu-id="d489e-166">String</span></span>|<span data-ttu-id="d489e-167">Категория аудита.</span><span class="sxs-lookup"><span data-stu-id="d489e-167">Audit category.</span></span>|



## <a name="response"></a><span data-ttu-id="d489e-168">Отклик</span><span class="sxs-lookup"><span data-stu-id="d489e-168">Response</span></span>
<span data-ttu-id="d489e-169">В случае успешного выполнения этот метод возвращает код отклика `201 Created` и объект [auditEvent](../resources/intune-auditing-auditevent.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="d489e-169">If successful, this method returns a `201 Created` response code and a [auditEvent](../resources/intune-auditing-auditevent.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d489e-170">Пример</span><span class="sxs-lookup"><span data-stu-id="d489e-170">Example</span></span>

### <a name="request"></a><span data-ttu-id="d489e-171">Запрос</span><span class="sxs-lookup"><span data-stu-id="d489e-171">Request</span></span>
<span data-ttu-id="d489e-172">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="d489e-172">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/auditEvents
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

### <a name="response"></a><span data-ttu-id="d489e-173">Отклик</span><span class="sxs-lookup"><span data-stu-id="d489e-173">Response</span></span>
<span data-ttu-id="d489e-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="d489e-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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




