---
title: Обновление roleScopeTag
description: Обновление свойства объекта roleScopeTag.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 6b05ba0be4e91bd9f4cb39ae316048f1f85194ab
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29404815"
---
# <a name="update-rolescopetag"></a><span data-ttu-id="71187-103">Обновление roleScopeTag</span><span class="sxs-lookup"><span data-stu-id="71187-103">Update roleScopeTag</span></span>

> <span data-ttu-id="71187-104">**Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="71187-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="71187-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="71187-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="71187-106">**Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="71187-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="71187-107">Обновление свойства объекта [roleScopeTag](../resources/intune-rbac-rolescopetag.md) .</span><span class="sxs-lookup"><span data-stu-id="71187-107">Update the properties of a [roleScopeTag](../resources/intune-rbac-rolescopetag.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="71187-108">Предварительные требования</span><span class="sxs-lookup"><span data-stu-id="71187-108">Prerequisites</span></span>
<span data-ttu-id="71187-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="71187-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="71187-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="71187-111">Permission type</span></span>|<span data-ttu-id="71187-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="71187-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="71187-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="71187-113">Delegated (work or school account)</span></span>|<span data-ttu-id="71187-114">DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="71187-114">DeviceManagementRBAC.ReadWrite.All</span></span>|
|<span data-ttu-id="71187-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="71187-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="71187-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="71187-116">Not supported.</span></span>|
|<span data-ttu-id="71187-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="71187-117">Application</span></span>|<span data-ttu-id="71187-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="71187-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="71187-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="71187-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/roleScopeTags/{roleScopeTagId}
PATCH /deviceManagement/roleDefinitions/{roleDefinitionId}/roleAssignments/{roleAssignmentId}/microsoft.graph.deviceAndAppManagementRoleAssignment/roleScopeTags/{roleScopeTagId}
```

## <a name="request-headers"></a><span data-ttu-id="71187-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="71187-120">Request headers</span></span>
|<span data-ttu-id="71187-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="71187-121">Header</span></span>|<span data-ttu-id="71187-122">Значение</span><span class="sxs-lookup"><span data-stu-id="71187-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="71187-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="71187-123">Authorization</span></span>|<span data-ttu-id="71187-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="71187-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="71187-125">Accept</span><span class="sxs-lookup"><span data-stu-id="71187-125">Accept</span></span>|<span data-ttu-id="71187-126">application/json</span><span class="sxs-lookup"><span data-stu-id="71187-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="71187-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="71187-127">Request body</span></span>
<span data-ttu-id="71187-128">В тексте запроса укажите представление JSON для объекта [roleScopeTag](../resources/intune-rbac-rolescopetag.md) .</span><span class="sxs-lookup"><span data-stu-id="71187-128">In the request body, supply a JSON representation for the [roleScopeTag](../resources/intune-rbac-rolescopetag.md) object.</span></span>

<span data-ttu-id="71187-129">В следующей таблице показаны свойства, которые необходимы для создания [roleScopeTag](../resources/intune-rbac-rolescopetag.md).</span><span class="sxs-lookup"><span data-stu-id="71187-129">The following table shows the properties that are required when you create the [roleScopeTag](../resources/intune-rbac-rolescopetag.md).</span></span>

|<span data-ttu-id="71187-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="71187-130">Property</span></span>|<span data-ttu-id="71187-131">Тип</span><span class="sxs-lookup"><span data-stu-id="71187-131">Type</span></span>|<span data-ttu-id="71187-132">Описание</span><span class="sxs-lookup"><span data-stu-id="71187-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="71187-133">id</span><span class="sxs-lookup"><span data-stu-id="71187-133">id</span></span>|<span data-ttu-id="71187-134">String</span><span class="sxs-lookup"><span data-stu-id="71187-134">String</span></span>|<span data-ttu-id="71187-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="71187-135">Key of the entity.</span></span> <span data-ttu-id="71187-136">Это свойство доступно только для чтения и создается автоматически.</span><span class="sxs-lookup"><span data-stu-id="71187-136">This is read-only and automatically generated.</span></span>|
|<span data-ttu-id="71187-137">displayName</span><span class="sxs-lookup"><span data-stu-id="71187-137">displayName</span></span>|<span data-ttu-id="71187-138">String</span><span class="sxs-lookup"><span data-stu-id="71187-138">String</span></span>|<span data-ttu-id="71187-139">Отображение или понятное имя тега область роли.</span><span class="sxs-lookup"><span data-stu-id="71187-139">The display or friendly name of the Role Scope Tag.</span></span>|
|<span data-ttu-id="71187-140">description</span><span class="sxs-lookup"><span data-stu-id="71187-140">description</span></span>|<span data-ttu-id="71187-141">String</span><span class="sxs-lookup"><span data-stu-id="71187-141">String</span></span>|<span data-ttu-id="71187-142">Описание тег область роли.</span><span class="sxs-lookup"><span data-stu-id="71187-142">Description of the Role Scope Tag.</span></span>|



## <a name="response"></a><span data-ttu-id="71187-143">Отклик</span><span class="sxs-lookup"><span data-stu-id="71187-143">Response</span></span>
<span data-ttu-id="71187-144">Успешно завершена, этот метод возвращает `200 OK` код ответа и обновленные [roleScopeTag](../resources/intune-rbac-rolescopetag.md) объекта в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="71187-144">If successful, this method returns a `200 OK` response code and an updated [roleScopeTag](../resources/intune-rbac-rolescopetag.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="71187-145">Пример</span><span class="sxs-lookup"><span data-stu-id="71187-145">Example</span></span>

### <a name="request"></a><span data-ttu-id="71187-146">Запрос</span><span class="sxs-lookup"><span data-stu-id="71187-146">Request</span></span>
<span data-ttu-id="71187-147">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="71187-147">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="71187-148">Отклик</span><span class="sxs-lookup"><span data-stu-id="71187-148">Response</span></span>
<span data-ttu-id="71187-p104">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="71187-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




