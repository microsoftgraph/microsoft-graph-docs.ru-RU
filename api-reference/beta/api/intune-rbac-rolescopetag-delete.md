---
title: Удаление Ролескопетаг
description: Удаляет объект Ролескопетаг.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: e58885ca37e0b8630e2fadba24428bbb419a32e1
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/14/2019
ms.locfileid: "34988386"
---
# <a name="delete-rolescopetag"></a><span data-ttu-id="b8126-103">Удаление Ролескопетаг</span><span class="sxs-lookup"><span data-stu-id="b8126-103">Delete roleScopeTag</span></span>

> <span data-ttu-id="b8126-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b8126-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b8126-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="b8126-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b8126-106">Удаляет объект [ролескопетаг](../resources/intune-rbac-rolescopetag.md).</span><span class="sxs-lookup"><span data-stu-id="b8126-106">Deletes a [roleScopeTag](../resources/intune-rbac-rolescopetag.md).</span></span>

## <a name="prerequisites"></a><span data-ttu-id="b8126-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="b8126-107">Prerequisites</span></span>
<span data-ttu-id="b8126-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b8126-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b8126-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="b8126-110">Permission type</span></span>|<span data-ttu-id="b8126-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="b8126-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b8126-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="b8126-112">Delegated (work or school account)</span></span>|<span data-ttu-id="b8126-113">DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b8126-113">DeviceManagementRBAC.ReadWrite.All</span></span>|
|<span data-ttu-id="b8126-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="b8126-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b8126-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b8126-115">Not supported.</span></span>|
|<span data-ttu-id="b8126-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="b8126-116">Application</span></span>|<span data-ttu-id="b8126-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b8126-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="b8126-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="b8126-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /deviceManagement/roleScopeTags/{roleScopeTagId}
DELETE /deviceManagement/roleDefinitions/{roleDefinitionId}/roleAssignments/{roleAssignmentId}/microsoft.graph.deviceAndAppManagementRoleAssignment/roleScopeTags/{roleScopeTagId}
```

## <a name="request-headers"></a><span data-ttu-id="b8126-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="b8126-119">Request headers</span></span>
|<span data-ttu-id="b8126-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="b8126-120">Header</span></span>|<span data-ttu-id="b8126-121">Значение</span><span class="sxs-lookup"><span data-stu-id="b8126-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b8126-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="b8126-122">Authorization</span></span>|<span data-ttu-id="b8126-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="b8126-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b8126-124">Accept</span><span class="sxs-lookup"><span data-stu-id="b8126-124">Accept</span></span>|<span data-ttu-id="b8126-125">application/json</span><span class="sxs-lookup"><span data-stu-id="b8126-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b8126-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="b8126-126">Request body</span></span>
<span data-ttu-id="b8126-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="b8126-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b8126-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="b8126-128">Response</span></span>
<span data-ttu-id="b8126-129">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="b8126-129">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="b8126-130">Пример</span><span class="sxs-lookup"><span data-stu-id="b8126-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="b8126-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="b8126-131">Request</span></span>
<span data-ttu-id="b8126-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="b8126-132">Here is an example of the request.</span></span>
``` http
DELETE https://graph.microsoft.com/beta/deviceManagement/roleScopeTags/{roleScopeTagId}
```

### <a name="response"></a><span data-ttu-id="b8126-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="b8126-133">Response</span></span>
<span data-ttu-id="b8126-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="b8126-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```





