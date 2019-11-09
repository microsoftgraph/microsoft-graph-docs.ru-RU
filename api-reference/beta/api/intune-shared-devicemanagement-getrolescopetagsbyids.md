---
title: Функция Жетролескопетагсбидс
description: Пока не задокументировано.
author: rolyon
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 2d6ab4ff00b136885f78f07830717653b59e0bcd
ms.sourcegitcommit: 5b1fad41067629d0e9f87746328664bb248f754f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/09/2019
ms.locfileid: "38086055"
---
# <a name="getrolescopetagsbyids-function"></a><span data-ttu-id="8f79e-103">Функция Жетролескопетагсбидс</span><span class="sxs-lookup"><span data-stu-id="8f79e-103">getRoleScopeTagsByIds function</span></span>

> <span data-ttu-id="8f79e-104">**Важно!** API в версии/Beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="8f79e-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="8f79e-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8f79e-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="8f79e-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="8f79e-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8f79e-107">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="8f79e-107">Not yet documented</span></span>
## <a name="prerequisites"></a><span data-ttu-id="8f79e-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="8f79e-108">Prerequisites</span></span>
<span data-ttu-id="8f79e-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8f79e-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8f79e-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="8f79e-111">Permission type</span></span>|<span data-ttu-id="8f79e-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="8f79e-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8f79e-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="8f79e-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="8f79e-114">&nbsp; &nbsp; **Управление доступом на основе ролей (RBAC)**</span><span class="sxs-lookup"><span data-stu-id="8f79e-114">&nbsp; &nbsp; **Role-based access control (RBAC)**</span></span> | <span data-ttu-id="8f79e-115">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span><span class="sxs-lookup"><span data-stu-id="8f79e-115">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span></span>|
|<span data-ttu-id="8f79e-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="8f79e-116">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8f79e-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8f79e-117">Not supported.</span></span>|
|<span data-ttu-id="8f79e-118">Для приложений</span><span class="sxs-lookup"><span data-stu-id="8f79e-118">Application</span></span>||
| <span data-ttu-id="8f79e-119">&nbsp; &nbsp; **Управление доступом на основе ролей (RBAC)**</span><span class="sxs-lookup"><span data-stu-id="8f79e-119">&nbsp; &nbsp; **Role-based access control (RBAC)**</span></span> | <span data-ttu-id="8f79e-120">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span><span class="sxs-lookup"><span data-stu-id="8f79e-120">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="8f79e-121">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="8f79e-121">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/getRoleScopeTagsByIds
```

## <a name="request-headers"></a><span data-ttu-id="8f79e-122">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="8f79e-122">Request headers</span></span>
|<span data-ttu-id="8f79e-123">Заголовок</span><span class="sxs-lookup"><span data-stu-id="8f79e-123">Header</span></span>|<span data-ttu-id="8f79e-124">Значение</span><span class="sxs-lookup"><span data-stu-id="8f79e-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="8f79e-125">Авторизация</span><span class="sxs-lookup"><span data-stu-id="8f79e-125">Authorization</span></span>|<span data-ttu-id="8f79e-126">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="8f79e-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="8f79e-127">Accept</span><span class="sxs-lookup"><span data-stu-id="8f79e-127">Accept</span></span>|<span data-ttu-id="8f79e-128">application/json</span><span class="sxs-lookup"><span data-stu-id="8f79e-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="8f79e-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="8f79e-129">Request body</span></span>
<span data-ttu-id="8f79e-130">В URL-адресе запроса укажите перечисленные ниже параметры запроса и их значения.</span><span class="sxs-lookup"><span data-stu-id="8f79e-130">In the request URL, provide the following query parameters with values.</span></span>
<span data-ttu-id="8f79e-131">В приведенной ниже таблице указаны параметры, которые можно использовать с этой функцией.</span><span class="sxs-lookup"><span data-stu-id="8f79e-131">The following table shows the parameters that can be used with this function.</span></span>

|<span data-ttu-id="8f79e-132">Свойство</span><span class="sxs-lookup"><span data-stu-id="8f79e-132">Property</span></span>|<span data-ttu-id="8f79e-133">Тип</span><span class="sxs-lookup"><span data-stu-id="8f79e-133">Type</span></span>|<span data-ttu-id="8f79e-134">Описание</span><span class="sxs-lookup"><span data-stu-id="8f79e-134">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8f79e-135">ids</span><span class="sxs-lookup"><span data-stu-id="8f79e-135">ids</span></span>|<span data-ttu-id="8f79e-136">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="8f79e-136">String collection</span></span>|<span data-ttu-id="8f79e-137">Н/Д</span><span class="sxs-lookup"><span data-stu-id="8f79e-137">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="8f79e-138">Ответ</span><span class="sxs-lookup"><span data-stu-id="8f79e-138">Response</span></span>
<span data-ttu-id="8f79e-139">В случае успеха эта функция возвращает код `200 OK` отклика и коллекцию [ролескопетаг](../resources/intune-rbac-rolescopetag.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="8f79e-139">If successful, this function returns a `200 OK` response code and a [roleScopeTag](../resources/intune-rbac-rolescopetag.md) collection in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8f79e-140">Пример</span><span class="sxs-lookup"><span data-stu-id="8f79e-140">Example</span></span>
### <a name="request"></a><span data-ttu-id="8f79e-141">Запрос</span><span class="sxs-lookup"><span data-stu-id="8f79e-141">Request</span></span>
<span data-ttu-id="8f79e-142">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="8f79e-142">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/getRoleScopeTagsByIds(ids=[
  "Ids value"
])
```

### <a name="response"></a><span data-ttu-id="8f79e-143">Отклик</span><span class="sxs-lookup"><span data-stu-id="8f79e-143">Response</span></span>
<span data-ttu-id="8f79e-p104">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="8f79e-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 231

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.roleScopeTag",
      "id": "9ed1e179-e179-9ed1-79e1-d19e79e1d19e",
      "displayName": "Display Name value",
      "description": "Description value"
    }
  ]
}
```












