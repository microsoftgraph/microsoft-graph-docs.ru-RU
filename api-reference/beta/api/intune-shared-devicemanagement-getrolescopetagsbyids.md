---
title: функция getRoleScopeTagsByIds
description: Н/Д
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 764bfd10fdfde445d38dbf5eb4f2552f02a8231f
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29403877"
---
# <a name="getrolescopetagsbyids-function"></a><span data-ttu-id="ede89-103">функция getRoleScopeTagsByIds</span><span class="sxs-lookup"><span data-stu-id="ede89-103">getRoleScopeTagsByIds function</span></span>

> <span data-ttu-id="ede89-104">**Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="ede89-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="ede89-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ede89-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="ede89-106">**Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="ede89-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ede89-107">Н/Д</span><span class="sxs-lookup"><span data-stu-id="ede89-107">Not yet documented</span></span>
## <a name="prerequisites"></a><span data-ttu-id="ede89-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="ede89-108">Prerequisites</span></span>
<span data-ttu-id="ede89-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ede89-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ede89-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ede89-111">Permission type</span></span>|<span data-ttu-id="ede89-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="ede89-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ede89-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ede89-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="ede89-114">&nbsp;&nbsp; **Управления доступом на основе ролей (RBAC)**</span><span class="sxs-lookup"><span data-stu-id="ede89-114">&nbsp; &nbsp; **Role-based access control (RBAC)**</span></span> | <span data-ttu-id="ede89-115">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span><span class="sxs-lookup"><span data-stu-id="ede89-115">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span></span>|
|<span data-ttu-id="ede89-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ede89-116">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ede89-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ede89-117">Not supported.</span></span>|
|<span data-ttu-id="ede89-118">Для приложений</span><span class="sxs-lookup"><span data-stu-id="ede89-118">Application</span></span>|<span data-ttu-id="ede89-119">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ede89-119">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="ede89-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ede89-120">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/getRoleScopeTagsByIds
```

## <a name="request-headers"></a><span data-ttu-id="ede89-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="ede89-121">Request headers</span></span>
|<span data-ttu-id="ede89-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="ede89-122">Header</span></span>|<span data-ttu-id="ede89-123">Значение</span><span class="sxs-lookup"><span data-stu-id="ede89-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ede89-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="ede89-124">Authorization</span></span>|<span data-ttu-id="ede89-125">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="ede89-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ede89-126">Accept</span><span class="sxs-lookup"><span data-stu-id="ede89-126">Accept</span></span>|<span data-ttu-id="ede89-127">application/json</span><span class="sxs-lookup"><span data-stu-id="ede89-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ede89-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="ede89-128">Request body</span></span>
<span data-ttu-id="ede89-129">В URL-адресе запроса укажите перечисленные ниже параметры запроса и их значения.</span><span class="sxs-lookup"><span data-stu-id="ede89-129">In the request URL, provide the following query parameters with values.</span></span>
<span data-ttu-id="ede89-130">В приведенной ниже таблице указаны параметры, которые можно использовать с этой функцией.</span><span class="sxs-lookup"><span data-stu-id="ede89-130">The following table shows the parameters that can be used with this function.</span></span>

|<span data-ttu-id="ede89-131">Свойство</span><span class="sxs-lookup"><span data-stu-id="ede89-131">Property</span></span>|<span data-ttu-id="ede89-132">Тип</span><span class="sxs-lookup"><span data-stu-id="ede89-132">Type</span></span>|<span data-ttu-id="ede89-133">Описание</span><span class="sxs-lookup"><span data-stu-id="ede89-133">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ede89-134">ids</span><span class="sxs-lookup"><span data-stu-id="ede89-134">ids</span></span>|<span data-ttu-id="ede89-135">Коллекция объектов string</span><span class="sxs-lookup"><span data-stu-id="ede89-135">String collection</span></span>|<span data-ttu-id="ede89-136">Н/Д</span><span class="sxs-lookup"><span data-stu-id="ede89-136">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="ede89-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="ede89-137">Response</span></span>
<span data-ttu-id="ede89-138">Если успешно завершена, эта функция возвращает `200 OK` код ответа и семейства [roleScopeTag](../resources/intune-rbac-rolescopetag.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="ede89-138">If successful, this function returns a `200 OK` response code and a [roleScopeTag](../resources/intune-rbac-rolescopetag.md) collection in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ede89-139">Пример</span><span class="sxs-lookup"><span data-stu-id="ede89-139">Example</span></span>
### <a name="request"></a><span data-ttu-id="ede89-140">Запрос</span><span class="sxs-lookup"><span data-stu-id="ede89-140">Request</span></span>
<span data-ttu-id="ede89-141">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="ede89-141">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/getRoleScopeTagsByIds(ids=[
  "Ids value"
])
```

### <a name="response"></a><span data-ttu-id="ede89-142">Отклик</span><span class="sxs-lookup"><span data-stu-id="ede89-142">Response</span></span>
<span data-ttu-id="ede89-p104">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="ede89-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



