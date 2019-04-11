---
title: Update auditEvent
description: Обновление свойств объекта auditEvent.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: cfe4e0dce5b85738ccf586ef3b739268badb3cc7
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/11/2019
ms.locfileid: "31776768"
---
# <a name="update-auditevent"></a><span data-ttu-id="b3495-103">Update auditEvent</span><span class="sxs-lookup"><span data-stu-id="b3495-103">Update auditEvent</span></span>

> <span data-ttu-id="b3495-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b3495-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b3495-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="b3495-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b3495-106">Обновление свойств объекта [auditEvent](../resources/intune-auditing-auditevent.md).</span><span class="sxs-lookup"><span data-stu-id="b3495-106">Update the properties of a [auditEvent](../resources/intune-auditing-auditevent.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="b3495-107">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="b3495-107">Prerequisites</span></span>
<span data-ttu-id="b3495-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b3495-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b3495-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="b3495-110">Permission type</span></span>|<span data-ttu-id="b3495-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="b3495-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b3495-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="b3495-112">Delegated (work or school account)</span></span>|<span data-ttu-id="b3495-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b3495-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="b3495-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="b3495-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b3495-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b3495-115">Not supported.</span></span>|
|<span data-ttu-id="b3495-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="b3495-116">Application</span></span>|<span data-ttu-id="b3495-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b3495-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="b3495-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="b3495-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/auditEvents/{auditEventId}
```

## <a name="request-headers"></a><span data-ttu-id="b3495-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="b3495-119">Request headers</span></span>
|<span data-ttu-id="b3495-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="b3495-120">Header</span></span>|<span data-ttu-id="b3495-121">Значение</span><span class="sxs-lookup"><span data-stu-id="b3495-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b3495-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="b3495-122">Authorization</span></span>|<span data-ttu-id="b3495-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="b3495-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b3495-124">Accept</span><span class="sxs-lookup"><span data-stu-id="b3495-124">Accept</span></span>|<span data-ttu-id="b3495-125">application/json</span><span class="sxs-lookup"><span data-stu-id="b3495-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b3495-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="b3495-126">Request body</span></span>
<span data-ttu-id="b3495-127">В теле запроса добавьте представление объекта [auditEvent](../resources/intune-auditing-auditevent.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="b3495-127">In the request body, supply a JSON representation for the [auditEvent](../resources/intune-auditing-auditevent.md) object.</span></span>

<span data-ttu-id="b3495-128">Ниже показаны свойства, которые необходимо указывать при создании объекта [auditEvent](../resources/intune-auditing-auditevent.md).</span><span class="sxs-lookup"><span data-stu-id="b3495-128">The following table shows the properties that are required when you create the [auditEvent](../resources/intune-auditing-auditevent.md).</span></span>

|<span data-ttu-id="b3495-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="b3495-129">Property</span></span>|<span data-ttu-id="b3495-130">Тип</span><span class="sxs-lookup"><span data-stu-id="b3495-130">Type</span></span>|<span data-ttu-id="b3495-131">Описание</span><span class="sxs-lookup"><span data-stu-id="b3495-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b3495-132">id</span><span class="sxs-lookup"><span data-stu-id="b3495-132">id</span></span>|<span data-ttu-id="b3495-133">String</span><span class="sxs-lookup"><span data-stu-id="b3495-133">String</span></span>|<span data-ttu-id="b3495-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="b3495-134">Key of the entity.</span></span>|
|<span data-ttu-id="b3495-135">displayName</span><span class="sxs-lookup"><span data-stu-id="b3495-135">displayName</span></span>|<span data-ttu-id="b3495-136">Строка</span><span class="sxs-lookup"><span data-stu-id="b3495-136">String</span></span>|<span data-ttu-id="b3495-137">Отображаемое имя события.</span><span class="sxs-lookup"><span data-stu-id="b3495-137">Event display name.</span></span>|
|<span data-ttu-id="b3495-138">componentName</span><span class="sxs-lookup"><span data-stu-id="b3495-138">componentName</span></span>|<span data-ttu-id="b3495-139">String</span><span class="sxs-lookup"><span data-stu-id="b3495-139">String</span></span>|<span data-ttu-id="b3495-140">Имя компонента.</span><span class="sxs-lookup"><span data-stu-id="b3495-140">Component name.</span></span>|
|<span data-ttu-id="b3495-141">actor</span><span class="sxs-lookup"><span data-stu-id="b3495-141">actor</span></span>|[<span data-ttu-id="b3495-142">auditActor</span><span class="sxs-lookup"><span data-stu-id="b3495-142">auditActor</span></span>](../resources/intune-auditing-auditactor.md)|<span data-ttu-id="b3495-143">Пользователь AAD и приложение, связанные с событием аудита.</span><span class="sxs-lookup"><span data-stu-id="b3495-143">AAD user and application that are associated with the audit event.</span></span>|
|<span data-ttu-id="b3495-144">activity</span><span class="sxs-lookup"><span data-stu-id="b3495-144">activity</span></span>|<span data-ttu-id="b3495-145">String</span><span class="sxs-lookup"><span data-stu-id="b3495-145">String</span></span>|<span data-ttu-id="b3495-146">Понятное имя действия.</span><span class="sxs-lookup"><span data-stu-id="b3495-146">Friendly name of the activity.</span></span>|
|<span data-ttu-id="b3495-147">activityDateTime</span><span class="sxs-lookup"><span data-stu-id="b3495-147">activityDateTime</span></span>|<span data-ttu-id="b3495-148">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b3495-148">DateTimeOffset</span></span>|<span data-ttu-id="b3495-149">Дата и время выполнения действия (в формате UTC).</span><span class="sxs-lookup"><span data-stu-id="b3495-149">The date time in UTC when the activity was performed.</span></span>|
|<span data-ttu-id="b3495-150">activityType</span><span class="sxs-lookup"><span data-stu-id="b3495-150">activityType</span></span>|<span data-ttu-id="b3495-151">String</span><span class="sxs-lookup"><span data-stu-id="b3495-151">String</span></span>|<span data-ttu-id="b3495-152">Тип выполненного действия.</span><span class="sxs-lookup"><span data-stu-id="b3495-152">The type of activity that was being performed.</span></span>|
|<span data-ttu-id="b3495-153">activityOperationType</span><span class="sxs-lookup"><span data-stu-id="b3495-153">activityOperationType</span></span>|<span data-ttu-id="b3495-154">String</span><span class="sxs-lookup"><span data-stu-id="b3495-154">String</span></span>|<span data-ttu-id="b3495-155">Тип операции HTTP для действия.</span><span class="sxs-lookup"><span data-stu-id="b3495-155">The HTTP operation type of the activity.</span></span>|
|<span data-ttu-id="b3495-156">activityResult</span><span class="sxs-lookup"><span data-stu-id="b3495-156">activityResult</span></span>|<span data-ttu-id="b3495-157">String</span><span class="sxs-lookup"><span data-stu-id="b3495-157">String</span></span>|<span data-ttu-id="b3495-158">Результат действия.</span><span class="sxs-lookup"><span data-stu-id="b3495-158">The result of the activity.</span></span>|
|<span data-ttu-id="b3495-159">correlationId</span><span class="sxs-lookup"><span data-stu-id="b3495-159">correlationId</span></span>|<span data-ttu-id="b3495-160">Guid</span><span class="sxs-lookup"><span data-stu-id="b3495-160">Guid</span></span>|<span data-ttu-id="b3495-161">ИД клиентского запроса, используемый для согласования действий в системе.</span><span class="sxs-lookup"><span data-stu-id="b3495-161">The client request Id that is used to correlate activity within the system.</span></span>|
|<span data-ttu-id="b3495-162">resources</span><span class="sxs-lookup"><span data-stu-id="b3495-162">resources</span></span>|<span data-ttu-id="b3495-163">Коллекция [auditResource](../resources/intune-auditing-auditresource.md)</span><span class="sxs-lookup"><span data-stu-id="b3495-163">[auditResource](../resources/intune-auditing-auditresource.md) collection</span></span>|<span data-ttu-id="b3495-164">Изменяемые ресурсы.</span><span class="sxs-lookup"><span data-stu-id="b3495-164">Resources being modified.</span></span>|
|<span data-ttu-id="b3495-165">category</span><span class="sxs-lookup"><span data-stu-id="b3495-165">category</span></span>|<span data-ttu-id="b3495-166">String</span><span class="sxs-lookup"><span data-stu-id="b3495-166">String</span></span>|<span data-ttu-id="b3495-167">Категория аудита.</span><span class="sxs-lookup"><span data-stu-id="b3495-167">Audit category.</span></span>|



## <a name="response"></a><span data-ttu-id="b3495-168">Ответ</span><span class="sxs-lookup"><span data-stu-id="b3495-168">Response</span></span>
<span data-ttu-id="b3495-169">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и обновленный объект [auditEvent](../resources/intune-auditing-auditevent.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="b3495-169">If successful, this method returns a `200 OK` response code and an updated [auditEvent](../resources/intune-auditing-auditevent.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b3495-170">Пример</span><span class="sxs-lookup"><span data-stu-id="b3495-170">Example</span></span>

### <a name="request"></a><span data-ttu-id="b3495-171">Запрос</span><span class="sxs-lookup"><span data-stu-id="b3495-171">Request</span></span>
<span data-ttu-id="b3495-172">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="b3495-172">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/auditEvents/{auditEventId}
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

### <a name="response"></a><span data-ttu-id="b3495-173">Отклик</span><span class="sxs-lookup"><span data-stu-id="b3495-173">Response</span></span>
<span data-ttu-id="b3495-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="b3495-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





