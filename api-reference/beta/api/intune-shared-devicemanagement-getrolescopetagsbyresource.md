---
title: Функция Жетролескопетагсбиресаурце
description: Пока не задокументировано.
author: rolyon
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 6e33da50ab709d1441e7da619051b64466254a75
ms.sourcegitcommit: 5b1fad41067629d0e9f87746328664bb248f754f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/09/2019
ms.locfileid: "38086048"
---
# <a name="getrolescopetagsbyresource-function"></a><span data-ttu-id="bcadc-103">Функция Жетролескопетагсбиресаурце</span><span class="sxs-lookup"><span data-stu-id="bcadc-103">getRoleScopeTagsByResource function</span></span>

> <span data-ttu-id="bcadc-104">**Важно!** API в версии/Beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="bcadc-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="bcadc-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="bcadc-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="bcadc-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="bcadc-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="bcadc-107">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="bcadc-107">Not yet documented</span></span>
## <a name="prerequisites"></a><span data-ttu-id="bcadc-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="bcadc-108">Prerequisites</span></span>
<span data-ttu-id="bcadc-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="bcadc-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="bcadc-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="bcadc-111">Permission type</span></span>|<span data-ttu-id="bcadc-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="bcadc-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="bcadc-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="bcadc-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="bcadc-114">&nbsp; &nbsp; **Управление доступом на основе ролей (RBAC)**</span><span class="sxs-lookup"><span data-stu-id="bcadc-114">&nbsp; &nbsp; **Role-based access control (RBAC)**</span></span> | <span data-ttu-id="bcadc-115">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span><span class="sxs-lookup"><span data-stu-id="bcadc-115">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span></span>|
|<span data-ttu-id="bcadc-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="bcadc-116">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="bcadc-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="bcadc-117">Not supported.</span></span>|
|<span data-ttu-id="bcadc-118">Для приложений</span><span class="sxs-lookup"><span data-stu-id="bcadc-118">Application</span></span>||
| <span data-ttu-id="bcadc-119">&nbsp; &nbsp; **Управление доступом на основе ролей (RBAC)**</span><span class="sxs-lookup"><span data-stu-id="bcadc-119">&nbsp; &nbsp; **Role-based access control (RBAC)**</span></span> | <span data-ttu-id="bcadc-120">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span><span class="sxs-lookup"><span data-stu-id="bcadc-120">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="bcadc-121">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="bcadc-121">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/getRoleScopeTagsByResource
```

## <a name="request-headers"></a><span data-ttu-id="bcadc-122">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="bcadc-122">Request headers</span></span>
|<span data-ttu-id="bcadc-123">Заголовок</span><span class="sxs-lookup"><span data-stu-id="bcadc-123">Header</span></span>|<span data-ttu-id="bcadc-124">Значение</span><span class="sxs-lookup"><span data-stu-id="bcadc-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="bcadc-125">Авторизация</span><span class="sxs-lookup"><span data-stu-id="bcadc-125">Authorization</span></span>|<span data-ttu-id="bcadc-126">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="bcadc-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="bcadc-127">Accept</span><span class="sxs-lookup"><span data-stu-id="bcadc-127">Accept</span></span>|<span data-ttu-id="bcadc-128">application/json</span><span class="sxs-lookup"><span data-stu-id="bcadc-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="bcadc-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="bcadc-129">Request body</span></span>
<span data-ttu-id="bcadc-130">В URL-адресе запроса укажите перечисленные ниже параметры запроса и их значения.</span><span class="sxs-lookup"><span data-stu-id="bcadc-130">In the request URL, provide the following query parameters with values.</span></span>
<span data-ttu-id="bcadc-131">В приведенной ниже таблице указаны параметры, которые можно использовать с этой функцией.</span><span class="sxs-lookup"><span data-stu-id="bcadc-131">The following table shows the parameters that can be used with this function.</span></span>

|<span data-ttu-id="bcadc-132">Свойство</span><span class="sxs-lookup"><span data-stu-id="bcadc-132">Property</span></span>|<span data-ttu-id="bcadc-133">Тип</span><span class="sxs-lookup"><span data-stu-id="bcadc-133">Type</span></span>|<span data-ttu-id="bcadc-134">Описание</span><span class="sxs-lookup"><span data-stu-id="bcadc-134">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="bcadc-135">resource</span><span class="sxs-lookup"><span data-stu-id="bcadc-135">resource</span></span>|<span data-ttu-id="bcadc-136">String</span><span class="sxs-lookup"><span data-stu-id="bcadc-136">String</span></span>|<span data-ttu-id="bcadc-137">Н/Д</span><span class="sxs-lookup"><span data-stu-id="bcadc-137">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="bcadc-138">Ответ</span><span class="sxs-lookup"><span data-stu-id="bcadc-138">Response</span></span>
<span data-ttu-id="bcadc-139">В случае успеха эта функция возвращает код `200 OK` отклика и коллекцию [ролескопетаг](../resources/intune-rbac-rolescopetag.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="bcadc-139">If successful, this function returns a `200 OK` response code and a [roleScopeTag](../resources/intune-rbac-rolescopetag.md) collection in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="bcadc-140">Пример</span><span class="sxs-lookup"><span data-stu-id="bcadc-140">Example</span></span>
### <a name="request"></a><span data-ttu-id="bcadc-141">Запрос</span><span class="sxs-lookup"><span data-stu-id="bcadc-141">Request</span></span>
<span data-ttu-id="bcadc-142">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="bcadc-142">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/getRoleScopeTagsByResource(resource='parameterValue')
```

### <a name="response"></a><span data-ttu-id="bcadc-143">Отклик</span><span class="sxs-lookup"><span data-stu-id="bcadc-143">Response</span></span>
<span data-ttu-id="bcadc-p104">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="bcadc-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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












