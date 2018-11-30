---
title: Создание roleScopeTag
description: Создание нового объекта roleScopeTag.
ms.openlocfilehash: b2f42999c785786175e5a6fb4dfd2b510d148927
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27078347"
---
# <a name="create-rolescopetag"></a><span data-ttu-id="f7c1f-103">Создание roleScopeTag</span><span class="sxs-lookup"><span data-stu-id="f7c1f-103">Create roleScopeTag</span></span>

> <span data-ttu-id="f7c1f-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="f7c1f-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="f7c1f-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f7c1f-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="f7c1f-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="f7c1f-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="f7c1f-107">Создание нового объекта [roleScopeTag](../resources/intune-rbac-rolescopetag.md) .</span><span class="sxs-lookup"><span data-stu-id="f7c1f-107">Create a new [roleScopeTag](../resources/intune-rbac-rolescopetag.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="f7c1f-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="f7c1f-108">Prerequisites</span></span>
<span data-ttu-id="f7c1f-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f7c1f-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f7c1f-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f7c1f-111">Permission type</span></span>|<span data-ttu-id="f7c1f-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="f7c1f-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f7c1f-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f7c1f-113">Delegated (work or school account)</span></span>|<span data-ttu-id="f7c1f-114">DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f7c1f-114">DeviceManagementRBAC.ReadWrite.All</span></span>|
|<span data-ttu-id="f7c1f-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f7c1f-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f7c1f-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f7c1f-116">Not supported.</span></span>|
|<span data-ttu-id="f7c1f-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="f7c1f-117">Application</span></span>|<span data-ttu-id="f7c1f-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f7c1f-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="f7c1f-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f7c1f-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/roleScopeTags
POST /deviceManagement/roleDefinitions/{roleDefinitionId}/roleAssignments/{roleAssignmentId}/microsoft.graph.deviceAndAppManagementRoleAssignment/roleScopeTags
```

## <a name="request-headers"></a><span data-ttu-id="f7c1f-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="f7c1f-120">Request headers</span></span>
|<span data-ttu-id="f7c1f-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="f7c1f-121">Header</span></span>|<span data-ttu-id="f7c1f-122">Значение</span><span class="sxs-lookup"><span data-stu-id="f7c1f-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f7c1f-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="f7c1f-123">Authorization</span></span>|<span data-ttu-id="f7c1f-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="f7c1f-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f7c1f-125">Accept</span><span class="sxs-lookup"><span data-stu-id="f7c1f-125">Accept</span></span>|<span data-ttu-id="f7c1f-126">application/json</span><span class="sxs-lookup"><span data-stu-id="f7c1f-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f7c1f-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="f7c1f-127">Request body</span></span>
<span data-ttu-id="f7c1f-128">В тексте запроса укажите представление JSON для объекта roleScopeTag.</span><span class="sxs-lookup"><span data-stu-id="f7c1f-128">In the request body, supply a JSON representation for the roleScopeTag object.</span></span>

<span data-ttu-id="f7c1f-129">В следующей таблице показаны свойства, которые необходимы для создания roleScopeTag.</span><span class="sxs-lookup"><span data-stu-id="f7c1f-129">The following table shows the properties that are required when you create the roleScopeTag.</span></span>

|<span data-ttu-id="f7c1f-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="f7c1f-130">Property</span></span>|<span data-ttu-id="f7c1f-131">Тип</span><span class="sxs-lookup"><span data-stu-id="f7c1f-131">Type</span></span>|<span data-ttu-id="f7c1f-132">Описание</span><span class="sxs-lookup"><span data-stu-id="f7c1f-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f7c1f-133">id</span><span class="sxs-lookup"><span data-stu-id="f7c1f-133">id</span></span>|<span data-ttu-id="f7c1f-134">String</span><span class="sxs-lookup"><span data-stu-id="f7c1f-134">String</span></span>|<span data-ttu-id="f7c1f-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="f7c1f-135">Key of the entity.</span></span> <span data-ttu-id="f7c1f-136">Это свойство доступно только для чтения и создается автоматически.</span><span class="sxs-lookup"><span data-stu-id="f7c1f-136">This is read-only and automatically generated.</span></span>|
|<span data-ttu-id="f7c1f-137">displayName</span><span class="sxs-lookup"><span data-stu-id="f7c1f-137">displayName</span></span>|<span data-ttu-id="f7c1f-138">String</span><span class="sxs-lookup"><span data-stu-id="f7c1f-138">String</span></span>|<span data-ttu-id="f7c1f-139">Отображение или понятное имя тега область роли.</span><span class="sxs-lookup"><span data-stu-id="f7c1f-139">The display or friendly name of the Role Scope Tag.</span></span>|
|<span data-ttu-id="f7c1f-140">описание</span><span class="sxs-lookup"><span data-stu-id="f7c1f-140">description</span></span>|<span data-ttu-id="f7c1f-141">String</span><span class="sxs-lookup"><span data-stu-id="f7c1f-141">String</span></span>|<span data-ttu-id="f7c1f-142">Описание тег область роли.</span><span class="sxs-lookup"><span data-stu-id="f7c1f-142">Description of the Role Scope Tag.</span></span>|



## <a name="response"></a><span data-ttu-id="f7c1f-143">Ответ</span><span class="sxs-lookup"><span data-stu-id="f7c1f-143">Response</span></span>
<span data-ttu-id="f7c1f-144">Успешно завершена, этот метод возвращает `201 Created` код ответа и объект [roleScopeTag](../resources/intune-rbac-rolescopetag.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="f7c1f-144">If successful, this method returns a `201 Created` response code and a [roleScopeTag](../resources/intune-rbac-rolescopetag.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f7c1f-145">Пример</span><span class="sxs-lookup"><span data-stu-id="f7c1f-145">Example</span></span>
### <a name="request"></a><span data-ttu-id="f7c1f-146">Запрос</span><span class="sxs-lookup"><span data-stu-id="f7c1f-146">Request</span></span>
<span data-ttu-id="f7c1f-147">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="f7c1f-147">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/roleScopeTags
Content-type: application/json
Content-length: 133

{
  "@odata.type": "#microsoft.graph.roleScopeTag",
  "displayName": "Display Name value",
  "description": "Description value"
}
```

### <a name="response"></a><span data-ttu-id="f7c1f-148">Ответ</span><span class="sxs-lookup"><span data-stu-id="f7c1f-148">Response</span></span>
<span data-ttu-id="f7c1f-p104">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
</span><span class="sxs-lookup"><span data-stu-id="f7c1f-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 182

{
  "@odata.type": "#microsoft.graph.roleScopeTag",
  "id": "9ed1e179-e179-9ed1-79e1-d19e79e1d19e",
  "displayName": "Display Name value",
  "description": "Description value"
}
```





