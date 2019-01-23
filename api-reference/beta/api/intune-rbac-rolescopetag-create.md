---
title: Создание roleScopeTag
description: Создание нового объекта roleScopeTag.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 61476fa106661baa179ff5344b8e4ac891b5a3b7
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29422196"
---
# <a name="create-rolescopetag"></a><span data-ttu-id="ee704-103">Создание roleScopeTag</span><span class="sxs-lookup"><span data-stu-id="ee704-103">Create roleScopeTag</span></span>

> <span data-ttu-id="ee704-104">**Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="ee704-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="ee704-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ee704-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="ee704-106">**Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="ee704-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ee704-107">Создание нового объекта [roleScopeTag](../resources/intune-rbac-rolescopetag.md) .</span><span class="sxs-lookup"><span data-stu-id="ee704-107">Create a new [roleScopeTag](../resources/intune-rbac-rolescopetag.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="ee704-108">Предварительные требования</span><span class="sxs-lookup"><span data-stu-id="ee704-108">Prerequisites</span></span>
<span data-ttu-id="ee704-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="ee704-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="ee704-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ee704-111">Permission type</span></span>|<span data-ttu-id="ee704-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="ee704-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ee704-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ee704-113">Delegated (work or school account)</span></span>|<span data-ttu-id="ee704-114">DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ee704-114">DeviceManagementRBAC.ReadWrite.All</span></span>|
|<span data-ttu-id="ee704-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ee704-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ee704-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ee704-116">Not supported.</span></span>|
|<span data-ttu-id="ee704-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="ee704-117">Application</span></span>|<span data-ttu-id="ee704-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ee704-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="ee704-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ee704-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/roleScopeTags
POST /deviceManagement/roleDefinitions/{roleDefinitionId}/roleAssignments/{roleAssignmentId}/microsoft.graph.deviceAndAppManagementRoleAssignment/roleScopeTags
```

## <a name="request-headers"></a><span data-ttu-id="ee704-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="ee704-120">Request headers</span></span>
|<span data-ttu-id="ee704-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="ee704-121">Header</span></span>|<span data-ttu-id="ee704-122">Значение</span><span class="sxs-lookup"><span data-stu-id="ee704-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ee704-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="ee704-123">Authorization</span></span>|<span data-ttu-id="ee704-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="ee704-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ee704-125">Accept</span><span class="sxs-lookup"><span data-stu-id="ee704-125">Accept</span></span>|<span data-ttu-id="ee704-126">application/json</span><span class="sxs-lookup"><span data-stu-id="ee704-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ee704-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="ee704-127">Request body</span></span>
<span data-ttu-id="ee704-128">В тексте запроса укажите представление JSON для объекта roleScopeTag.</span><span class="sxs-lookup"><span data-stu-id="ee704-128">In the request body, supply a JSON representation for the roleScopeTag object.</span></span>

<span data-ttu-id="ee704-129">В следующей таблице показаны свойства, которые необходимы для создания roleScopeTag.</span><span class="sxs-lookup"><span data-stu-id="ee704-129">The following table shows the properties that are required when you create the roleScopeTag.</span></span>

|<span data-ttu-id="ee704-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="ee704-130">Property</span></span>|<span data-ttu-id="ee704-131">Тип</span><span class="sxs-lookup"><span data-stu-id="ee704-131">Type</span></span>|<span data-ttu-id="ee704-132">Описание</span><span class="sxs-lookup"><span data-stu-id="ee704-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ee704-133">id</span><span class="sxs-lookup"><span data-stu-id="ee704-133">id</span></span>|<span data-ttu-id="ee704-134">String</span><span class="sxs-lookup"><span data-stu-id="ee704-134">String</span></span>|<span data-ttu-id="ee704-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="ee704-135">Key of the entity.</span></span> <span data-ttu-id="ee704-136">Это свойство доступно только для чтения и создается автоматически.</span><span class="sxs-lookup"><span data-stu-id="ee704-136">This is read-only and automatically generated.</span></span>|
|<span data-ttu-id="ee704-137">displayName</span><span class="sxs-lookup"><span data-stu-id="ee704-137">displayName</span></span>|<span data-ttu-id="ee704-138">String</span><span class="sxs-lookup"><span data-stu-id="ee704-138">String</span></span>|<span data-ttu-id="ee704-139">Отображение или понятное имя тега область роли.</span><span class="sxs-lookup"><span data-stu-id="ee704-139">The display or friendly name of the Role Scope Tag.</span></span>|
|<span data-ttu-id="ee704-140">description</span><span class="sxs-lookup"><span data-stu-id="ee704-140">description</span></span>|<span data-ttu-id="ee704-141">String</span><span class="sxs-lookup"><span data-stu-id="ee704-141">String</span></span>|<span data-ttu-id="ee704-142">Описание тег область роли.</span><span class="sxs-lookup"><span data-stu-id="ee704-142">Description of the Role Scope Tag.</span></span>|



## <a name="response"></a><span data-ttu-id="ee704-143">Отклик</span><span class="sxs-lookup"><span data-stu-id="ee704-143">Response</span></span>
<span data-ttu-id="ee704-144">Успешно завершена, этот метод возвращает `201 Created` код ответа и объект [roleScopeTag](../resources/intune-rbac-rolescopetag.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="ee704-144">If successful, this method returns a `201 Created` response code and a [roleScopeTag](../resources/intune-rbac-rolescopetag.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ee704-145">Пример</span><span class="sxs-lookup"><span data-stu-id="ee704-145">Example</span></span>

### <a name="request"></a><span data-ttu-id="ee704-146">Запрос</span><span class="sxs-lookup"><span data-stu-id="ee704-146">Request</span></span>
<span data-ttu-id="ee704-147">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="ee704-147">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="ee704-148">Отклик</span><span class="sxs-lookup"><span data-stu-id="ee704-148">Response</span></span>
<span data-ttu-id="ee704-p104">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="ee704-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




