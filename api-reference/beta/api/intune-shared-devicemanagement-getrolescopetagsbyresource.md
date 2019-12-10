---
title: Функция Жетролескопетагсбиресаурце
description: Пока не задокументировано.
author: rolyon
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 61096e905093b76399fc6ca4342c0cfd32585f59
ms.sourcegitcommit: 53dd31d323319fbd2ff7afc51b55a46efb8c5be3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/10/2019
ms.locfileid: "39939972"
---
# <a name="getrolescopetagsbyresource-function"></a><span data-ttu-id="8ae5f-103">Функция Жетролескопетагсбиресаурце</span><span class="sxs-lookup"><span data-stu-id="8ae5f-103">getRoleScopeTagsByResource function</span></span>

> <span data-ttu-id="8ae5f-104">**Важно!** API в версии/Beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="8ae5f-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="8ae5f-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8ae5f-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="8ae5f-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="8ae5f-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8ae5f-107">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="8ae5f-107">Not yet documented</span></span>
## <a name="prerequisites"></a><span data-ttu-id="8ae5f-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="8ae5f-108">Prerequisites</span></span>
<span data-ttu-id="8ae5f-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8ae5f-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8ae5f-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="8ae5f-111">Permission type</span></span>|<span data-ttu-id="8ae5f-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="8ae5f-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8ae5f-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="8ae5f-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="8ae5f-114">&nbsp; &nbsp; **Управление доступом на основе ролей (RBAC)**</span><span class="sxs-lookup"><span data-stu-id="8ae5f-114">&nbsp; &nbsp; **Role-based access control (RBAC)**</span></span> | <span data-ttu-id="8ae5f-115">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span><span class="sxs-lookup"><span data-stu-id="8ae5f-115">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span></span>|
|<span data-ttu-id="8ae5f-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="8ae5f-116">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8ae5f-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8ae5f-117">Not supported.</span></span>|
|<span data-ttu-id="8ae5f-118">Для приложений</span><span class="sxs-lookup"><span data-stu-id="8ae5f-118">Application</span></span>||
| <span data-ttu-id="8ae5f-119">&nbsp; &nbsp; **Управление доступом на основе ролей (RBAC)**</span><span class="sxs-lookup"><span data-stu-id="8ae5f-119">&nbsp; &nbsp; **Role-based access control (RBAC)**</span></span> | <span data-ttu-id="8ae5f-120">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span><span class="sxs-lookup"><span data-stu-id="8ae5f-120">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="8ae5f-121">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="8ae5f-121">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/getRoleScopeTagsByResource
```

## <a name="request-headers"></a><span data-ttu-id="8ae5f-122">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="8ae5f-122">Request headers</span></span>
|<span data-ttu-id="8ae5f-123">Заголовок</span><span class="sxs-lookup"><span data-stu-id="8ae5f-123">Header</span></span>|<span data-ttu-id="8ae5f-124">Значение</span><span class="sxs-lookup"><span data-stu-id="8ae5f-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="8ae5f-125">Авторизация</span><span class="sxs-lookup"><span data-stu-id="8ae5f-125">Authorization</span></span>|<span data-ttu-id="8ae5f-126">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="8ae5f-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="8ae5f-127">Accept</span><span class="sxs-lookup"><span data-stu-id="8ae5f-127">Accept</span></span>|<span data-ttu-id="8ae5f-128">application/json</span><span class="sxs-lookup"><span data-stu-id="8ae5f-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="8ae5f-129">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="8ae5f-129">Request body</span></span>
<span data-ttu-id="8ae5f-130">В URL-адресе запроса укажите перечисленные ниже параметры запроса и их значения.</span><span class="sxs-lookup"><span data-stu-id="8ae5f-130">In the request URL, provide the following query parameters with values.</span></span>
<span data-ttu-id="8ae5f-131">В приведенной ниже таблице указаны параметры, которые можно использовать с этой функцией.</span><span class="sxs-lookup"><span data-stu-id="8ae5f-131">The following table shows the parameters that can be used with this function.</span></span>

|<span data-ttu-id="8ae5f-132">Свойство</span><span class="sxs-lookup"><span data-stu-id="8ae5f-132">Property</span></span>|<span data-ttu-id="8ae5f-133">Тип</span><span class="sxs-lookup"><span data-stu-id="8ae5f-133">Type</span></span>|<span data-ttu-id="8ae5f-134">Описание</span><span class="sxs-lookup"><span data-stu-id="8ae5f-134">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8ae5f-135">resource</span><span class="sxs-lookup"><span data-stu-id="8ae5f-135">resource</span></span>|<span data-ttu-id="8ae5f-136">String</span><span class="sxs-lookup"><span data-stu-id="8ae5f-136">String</span></span>|<span data-ttu-id="8ae5f-137">Н/Д</span><span class="sxs-lookup"><span data-stu-id="8ae5f-137">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="8ae5f-138">Ответ</span><span class="sxs-lookup"><span data-stu-id="8ae5f-138">Response</span></span>
<span data-ttu-id="8ae5f-139">В случае успеха эта функция возвращает код `200 OK` отклика и коллекцию [ролескопетаг](../resources/intune-rbac-rolescopetag.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="8ae5f-139">If successful, this function returns a `200 OK` response code and a [roleScopeTag](../resources/intune-rbac-rolescopetag.md) collection in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8ae5f-140">Пример</span><span class="sxs-lookup"><span data-stu-id="8ae5f-140">Example</span></span>
### <a name="request"></a><span data-ttu-id="8ae5f-141">Запрос</span><span class="sxs-lookup"><span data-stu-id="8ae5f-141">Request</span></span>
<span data-ttu-id="8ae5f-142">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="8ae5f-142">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/getRoleScopeTagsByResource(resource='parameterValue')
```

### <a name="response"></a><span data-ttu-id="8ae5f-143">Отклик</span><span class="sxs-lookup"><span data-stu-id="8ae5f-143">Response</span></span>
<span data-ttu-id="8ae5f-p104">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="8ae5f-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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











