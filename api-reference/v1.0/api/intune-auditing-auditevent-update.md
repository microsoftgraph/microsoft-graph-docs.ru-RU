---
title: Update auditEvent
description: Обновление свойств объекта auditEvent.
author: tfitzmac
ms.openlocfilehash: 631144a0192af20580cdbf108d3acf7daa3d82f7
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27310047"
---
# <a name="update-auditevent"></a><span data-ttu-id="fda46-103">Update auditEvent</span><span class="sxs-lookup"><span data-stu-id="fda46-103">Update auditEvent</span></span>

> <span data-ttu-id="fda46-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="fda46-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="fda46-105">Обновление свойств объекта [auditEvent](../resources/intune-auditing-auditevent.md).</span><span class="sxs-lookup"><span data-stu-id="fda46-105">Update the properties of a [auditEvent](../resources/intune-auditing-auditevent.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="fda46-106">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="fda46-106">Prerequisites</span></span>
<span data-ttu-id="fda46-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="fda46-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fda46-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="fda46-109">Permission type</span></span>|<span data-ttu-id="fda46-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="fda46-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="fda46-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="fda46-111">Delegated (work or school account)</span></span>|<span data-ttu-id="fda46-112">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fda46-112">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="fda46-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="fda46-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="fda46-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fda46-114">Not supported.</span></span>|
|<span data-ttu-id="fda46-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="fda46-115">Application</span></span>|<span data-ttu-id="fda46-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fda46-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="fda46-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="fda46-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/auditEvents/{auditEventId}
```

## <a name="request-headers"></a><span data-ttu-id="fda46-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="fda46-118">Request headers</span></span>
|<span data-ttu-id="fda46-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="fda46-119">Header</span></span>|<span data-ttu-id="fda46-120">Значение</span><span class="sxs-lookup"><span data-stu-id="fda46-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="fda46-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="fda46-121">Authorization</span></span>|<span data-ttu-id="fda46-122">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="fda46-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="fda46-123">Accept</span><span class="sxs-lookup"><span data-stu-id="fda46-123">Accept</span></span>|<span data-ttu-id="fda46-124">application/json</span><span class="sxs-lookup"><span data-stu-id="fda46-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="fda46-125">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="fda46-125">Request body</span></span>
<span data-ttu-id="fda46-126">В теле запроса добавьте представление объекта [auditEvent](../resources/intune-auditing-auditevent.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="fda46-126">In the request body, supply a JSON representation for the [auditEvent](../resources/intune-auditing-auditevent.md) object.</span></span>

<span data-ttu-id="fda46-127">Ниже показаны свойства, которые необходимо указывать при создании объекта [auditEvent](../resources/intune-auditing-auditevent.md).</span><span class="sxs-lookup"><span data-stu-id="fda46-127">The following table shows the properties that are required when you create the [auditEvent](../resources/intune-auditing-auditevent.md).</span></span>

|<span data-ttu-id="fda46-128">Свойство</span><span class="sxs-lookup"><span data-stu-id="fda46-128">Property</span></span>|<span data-ttu-id="fda46-129">Тип</span><span class="sxs-lookup"><span data-stu-id="fda46-129">Type</span></span>|<span data-ttu-id="fda46-130">Описание</span><span class="sxs-lookup"><span data-stu-id="fda46-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fda46-131">id</span><span class="sxs-lookup"><span data-stu-id="fda46-131">id</span></span>|<span data-ttu-id="fda46-132">Строка</span><span class="sxs-lookup"><span data-stu-id="fda46-132">String</span></span>|<span data-ttu-id="fda46-133">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="fda46-133">Key of the entity.</span></span>|
|<span data-ttu-id="fda46-134">displayName</span><span class="sxs-lookup"><span data-stu-id="fda46-134">displayName</span></span>|<span data-ttu-id="fda46-135">String</span><span class="sxs-lookup"><span data-stu-id="fda46-135">String</span></span>|<span data-ttu-id="fda46-136">Отображаемое имя события.</span><span class="sxs-lookup"><span data-stu-id="fda46-136">Event display name.</span></span>|
|<span data-ttu-id="fda46-137">componentName</span><span class="sxs-lookup"><span data-stu-id="fda46-137">componentName</span></span>|<span data-ttu-id="fda46-138">String</span><span class="sxs-lookup"><span data-stu-id="fda46-138">String</span></span>|<span data-ttu-id="fda46-139">Имя компонента.</span><span class="sxs-lookup"><span data-stu-id="fda46-139">Component name.</span></span>|
|<span data-ttu-id="fda46-140">actor</span><span class="sxs-lookup"><span data-stu-id="fda46-140">actor</span></span>|[<span data-ttu-id="fda46-141">auditActor</span><span class="sxs-lookup"><span data-stu-id="fda46-141">auditActor</span></span>](../resources/intune-auditing-auditactor.md)|<span data-ttu-id="fda46-142">Пользователь AAD и приложение, связанные с событием аудита.</span><span class="sxs-lookup"><span data-stu-id="fda46-142">AAD user and application that are associated with the audit event.</span></span>|
|<span data-ttu-id="fda46-143">activity</span><span class="sxs-lookup"><span data-stu-id="fda46-143">activity</span></span>|<span data-ttu-id="fda46-144">String</span><span class="sxs-lookup"><span data-stu-id="fda46-144">String</span></span>|<span data-ttu-id="fda46-145">Понятное имя действия.</span><span class="sxs-lookup"><span data-stu-id="fda46-145">Friendly name of the activity.</span></span>|
|<span data-ttu-id="fda46-146">activityDateTime</span><span class="sxs-lookup"><span data-stu-id="fda46-146">activityDateTime</span></span>|<span data-ttu-id="fda46-147">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="fda46-147">DateTimeOffset</span></span>|<span data-ttu-id="fda46-148">Дата и время выполнения действия (в формате UTC).</span><span class="sxs-lookup"><span data-stu-id="fda46-148">The date time in UTC when the activity was performed.</span></span>|
|<span data-ttu-id="fda46-149">activityType</span><span class="sxs-lookup"><span data-stu-id="fda46-149">activityType</span></span>|<span data-ttu-id="fda46-150">String</span><span class="sxs-lookup"><span data-stu-id="fda46-150">String</span></span>|<span data-ttu-id="fda46-151">Тип выполненного действия.</span><span class="sxs-lookup"><span data-stu-id="fda46-151">The type of activity that was being performed.</span></span>|
|<span data-ttu-id="fda46-152">activityOperationType</span><span class="sxs-lookup"><span data-stu-id="fda46-152">activityOperationType</span></span>|<span data-ttu-id="fda46-153">String</span><span class="sxs-lookup"><span data-stu-id="fda46-153">String</span></span>|<span data-ttu-id="fda46-154">Тип операции HTTP для действия.</span><span class="sxs-lookup"><span data-stu-id="fda46-154">The HTTP operation type of the activity.</span></span>|
|<span data-ttu-id="fda46-155">activityResult</span><span class="sxs-lookup"><span data-stu-id="fda46-155">activityResult</span></span>|<span data-ttu-id="fda46-156">String</span><span class="sxs-lookup"><span data-stu-id="fda46-156">String</span></span>|<span data-ttu-id="fda46-157">Результат действия.</span><span class="sxs-lookup"><span data-stu-id="fda46-157">The result of the activity.</span></span>|
|<span data-ttu-id="fda46-158">correlationId</span><span class="sxs-lookup"><span data-stu-id="fda46-158">correlationId</span></span>|<span data-ttu-id="fda46-159">Guid</span><span class="sxs-lookup"><span data-stu-id="fda46-159">Guid</span></span>|<span data-ttu-id="fda46-160">Идентификатор клиентского запроса, используемый для согласования действий в системе.</span><span class="sxs-lookup"><span data-stu-id="fda46-160">The client request Id that is used to correlate activity within the system.</span></span>|
|<span data-ttu-id="fda46-161">resources</span><span class="sxs-lookup"><span data-stu-id="fda46-161">resources</span></span>|<span data-ttu-id="fda46-162">Коллекция [auditResource](../resources/intune-auditing-auditresource.md)</span><span class="sxs-lookup"><span data-stu-id="fda46-162">[auditResource](../resources/intune-auditing-auditresource.md) collection</span></span>|<span data-ttu-id="fda46-163">Изменяемые ресурсы.</span><span class="sxs-lookup"><span data-stu-id="fda46-163">Resources being modified.</span></span>|
|<span data-ttu-id="fda46-164">category</span><span class="sxs-lookup"><span data-stu-id="fda46-164">category</span></span>|<span data-ttu-id="fda46-165">String</span><span class="sxs-lookup"><span data-stu-id="fda46-165">String</span></span>|<span data-ttu-id="fda46-166">Категория аудита.</span><span class="sxs-lookup"><span data-stu-id="fda46-166">Audit category.</span></span>|



## <a name="response"></a><span data-ttu-id="fda46-167">Ответ</span><span class="sxs-lookup"><span data-stu-id="fda46-167">Response</span></span>
<span data-ttu-id="fda46-168">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и обновленный объект [auditEvent](../resources/intune-auditing-auditevent.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="fda46-168">If successful, this method returns a `200 OK` response code and an updated [auditEvent](../resources/intune-auditing-auditevent.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="fda46-169">Пример</span><span class="sxs-lookup"><span data-stu-id="fda46-169">Example</span></span>
### <a name="request"></a><span data-ttu-id="fda46-170">Запрос</span><span class="sxs-lookup"><span data-stu-id="fda46-170">Request</span></span>
<span data-ttu-id="fda46-171">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="fda46-171">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="fda46-172">Ответ</span><span class="sxs-lookup"><span data-stu-id="fda46-172">Response</span></span>
<span data-ttu-id="fda46-p102">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="fda46-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



