---
title: Обновление Ролескопетаг
description: Обновление свойств объекта Ролескопетаг.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 7a0adb3e151eb4b9d54a7c83d886deb99ac23573
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/29/2019
ms.locfileid: "30959427"
---
# <a name="update-rolescopetag"></a><span data-ttu-id="f1583-103">Обновление Ролескопетаг</span><span class="sxs-lookup"><span data-stu-id="f1583-103">Update roleScopeTag</span></span>

> <span data-ttu-id="f1583-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f1583-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f1583-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="f1583-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f1583-106">Обновление свойств объекта [ролескопетаг](../resources/intune-rbac-rolescopetag.md) .</span><span class="sxs-lookup"><span data-stu-id="f1583-106">Update the properties of a [roleScopeTag](../resources/intune-rbac-rolescopetag.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f1583-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="f1583-107">Prerequisites</span></span>
<span data-ttu-id="f1583-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f1583-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f1583-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f1583-110">Permission type</span></span>|<span data-ttu-id="f1583-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="f1583-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f1583-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f1583-112">Delegated (work or school account)</span></span>|<span data-ttu-id="f1583-113">DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f1583-113">DeviceManagementRBAC.ReadWrite.All</span></span>|
|<span data-ttu-id="f1583-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f1583-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f1583-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f1583-115">Not supported.</span></span>|
|<span data-ttu-id="f1583-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="f1583-116">Application</span></span>|<span data-ttu-id="f1583-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f1583-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="f1583-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f1583-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/roleScopeTags/{roleScopeTagId}
PATCH /deviceManagement/roleDefinitions/{roleDefinitionId}/roleAssignments/{roleAssignmentId}/microsoft.graph.deviceAndAppManagementRoleAssignment/roleScopeTags/{roleScopeTagId}
```

## <a name="request-headers"></a><span data-ttu-id="f1583-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="f1583-119">Request headers</span></span>
|<span data-ttu-id="f1583-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="f1583-120">Header</span></span>|<span data-ttu-id="f1583-121">Значение</span><span class="sxs-lookup"><span data-stu-id="f1583-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f1583-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="f1583-122">Authorization</span></span>|<span data-ttu-id="f1583-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="f1583-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f1583-124">Accept</span><span class="sxs-lookup"><span data-stu-id="f1583-124">Accept</span></span>|<span data-ttu-id="f1583-125">application/json</span><span class="sxs-lookup"><span data-stu-id="f1583-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f1583-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="f1583-126">Request body</span></span>
<span data-ttu-id="f1583-127">В тексте запроса добавьте представление объекта [Ролескопетаг](../resources/intune-rbac-rolescopetag.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="f1583-127">In the request body, supply a JSON representation for the [roleScopeTag](../resources/intune-rbac-rolescopetag.md) object.</span></span>

<span data-ttu-id="f1583-128">В следующей таблице приведены свойства, необходимые при создании [ролескопетаг](../resources/intune-rbac-rolescopetag.md).</span><span class="sxs-lookup"><span data-stu-id="f1583-128">The following table shows the properties that are required when you create the [roleScopeTag](../resources/intune-rbac-rolescopetag.md).</span></span>

|<span data-ttu-id="f1583-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="f1583-129">Property</span></span>|<span data-ttu-id="f1583-130">Тип</span><span class="sxs-lookup"><span data-stu-id="f1583-130">Type</span></span>|<span data-ttu-id="f1583-131">Описание</span><span class="sxs-lookup"><span data-stu-id="f1583-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f1583-132">id</span><span class="sxs-lookup"><span data-stu-id="f1583-132">id</span></span>|<span data-ttu-id="f1583-133">Строка</span><span class="sxs-lookup"><span data-stu-id="f1583-133">String</span></span>|<span data-ttu-id="f1583-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="f1583-134">Key of the entity.</span></span> <span data-ttu-id="f1583-135">Это свойство доступно только для чтения и создается автоматически.</span><span class="sxs-lookup"><span data-stu-id="f1583-135">This is read-only and automatically generated.</span></span>|
|<span data-ttu-id="f1583-136">displayName</span><span class="sxs-lookup"><span data-stu-id="f1583-136">displayName</span></span>|<span data-ttu-id="f1583-137">String</span><span class="sxs-lookup"><span data-stu-id="f1583-137">String</span></span>|<span data-ttu-id="f1583-138">Отображаемое или понятное имя тега области применения роли.</span><span class="sxs-lookup"><span data-stu-id="f1583-138">The display or friendly name of the Role Scope Tag.</span></span>|
|<span data-ttu-id="f1583-139">description</span><span class="sxs-lookup"><span data-stu-id="f1583-139">description</span></span>|<span data-ttu-id="f1583-140">String</span><span class="sxs-lookup"><span data-stu-id="f1583-140">String</span></span>|<span data-ttu-id="f1583-141">Описание тега области применения роли.</span><span class="sxs-lookup"><span data-stu-id="f1583-141">Description of the Role Scope Tag.</span></span>|



## <a name="response"></a><span data-ttu-id="f1583-142">Отклик</span><span class="sxs-lookup"><span data-stu-id="f1583-142">Response</span></span>
<span data-ttu-id="f1583-143">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [ролескопетаг](../resources/intune-rbac-rolescopetag.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="f1583-143">If successful, this method returns a `200 OK` response code and an updated [roleScopeTag](../resources/intune-rbac-rolescopetag.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f1583-144">Пример</span><span class="sxs-lookup"><span data-stu-id="f1583-144">Example</span></span>

### <a name="request"></a><span data-ttu-id="f1583-145">Запрос</span><span class="sxs-lookup"><span data-stu-id="f1583-145">Request</span></span>
<span data-ttu-id="f1583-146">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="f1583-146">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/roleScopeTags/{roleScopeTagId}
Content-type: application/json
Content-length: 133

{
  "@odata.type": "#microsoft.graph.roleScopeTag",
  "displayName": "Display Name value",
  "description": "Description value"
}
```

### <a name="response"></a><span data-ttu-id="f1583-147">Отклик</span><span class="sxs-lookup"><span data-stu-id="f1583-147">Response</span></span>
<span data-ttu-id="f1583-p103">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="f1583-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 182

{
  "@odata.type": "#microsoft.graph.roleScopeTag",
  "id": "9ed1e179-e179-9ed1-79e1-d19e79e1d19e",
  "displayName": "Display Name value",
  "description": "Description value"
}
```




