---
title: Функция getManagedAppDiagnosticStatuses
description: Получает состояние диагностической проверки для определенного пользователя.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: c12d3f03fd608f23a94afcf4ac7a2a75a6d8f846
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36025801"
---
# <a name="getmanagedappdiagnosticstatuses-function"></a><span data-ttu-id="5a3e9-103">Функция getManagedAppDiagnosticStatuses</span><span class="sxs-lookup"><span data-stu-id="5a3e9-103">getManagedAppDiagnosticStatuses function</span></span>

> <span data-ttu-id="5a3e9-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="5a3e9-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5a3e9-105">Получает состояние диагностической проверки для определенного пользователя.</span><span class="sxs-lookup"><span data-stu-id="5a3e9-105">Gets diagnostics validation status for a given user.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="5a3e9-106">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="5a3e9-106">Prerequisites</span></span>
<span data-ttu-id="5a3e9-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5a3e9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5a3e9-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="5a3e9-109">Permission type</span></span>|<span data-ttu-id="5a3e9-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="5a3e9-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="5a3e9-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="5a3e9-111">Delegated (work or school account)</span></span>| <span data-ttu-id="5a3e9-112">_зависит от контекста_</span><span class="sxs-lookup"><span data-stu-id="5a3e9-112">_varies by context_</span></span>|
| <span data-ttu-id="5a3e9-113">&nbsp;&nbsp; MAM</span><span class="sxs-lookup"><span data-stu-id="5a3e9-113">&nbsp; &nbsp; MAM</span></span> | <span data-ttu-id="5a3e9-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="5a3e9-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span> |
|<span data-ttu-id="5a3e9-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="5a3e9-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5a3e9-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5a3e9-116">Not supported.</span></span>|
|<span data-ttu-id="5a3e9-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="5a3e9-117">Application</span></span>|<span data-ttu-id="5a3e9-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5a3e9-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="5a3e9-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="5a3e9-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /users/{usersId}/getManagedAppDiagnosticStatuses
```

## <a name="request-headers"></a><span data-ttu-id="5a3e9-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="5a3e9-120">Request headers</span></span>
|<span data-ttu-id="5a3e9-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="5a3e9-121">Header</span></span>|<span data-ttu-id="5a3e9-122">Значение</span><span class="sxs-lookup"><span data-stu-id="5a3e9-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="5a3e9-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="5a3e9-123">Authorization</span></span>|<span data-ttu-id="5a3e9-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="5a3e9-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="5a3e9-125">Accept</span><span class="sxs-lookup"><span data-stu-id="5a3e9-125">Accept</span></span>|<span data-ttu-id="5a3e9-126">application/json</span><span class="sxs-lookup"><span data-stu-id="5a3e9-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="5a3e9-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="5a3e9-127">Request body</span></span>
<span data-ttu-id="5a3e9-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="5a3e9-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="5a3e9-129">Ответ</span><span class="sxs-lookup"><span data-stu-id="5a3e9-129">Response</span></span>
<span data-ttu-id="5a3e9-130">При успешном выполнении эта функция возвращает код отклика `200 OK` и коллекцию [managedAppDiagnosticStatus](../resources/intune-mam-managedappdiagnosticstatus.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="5a3e9-130">If successful, this function returns a `200 OK` response code and a [managedAppDiagnosticStatus](../resources/intune-mam-managedappdiagnosticstatus.md) collection in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5a3e9-131">Пример</span><span class="sxs-lookup"><span data-stu-id="5a3e9-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="5a3e9-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="5a3e9-132">Request</span></span>
<span data-ttu-id="5a3e9-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="5a3e9-133">Here is an example of the request.</span></span>

``` http
GET https://graph.microsoft.com/v1.0/users/{usersId}/getManagedAppDiagnosticStatuses
```

### <a name="response"></a><span data-ttu-id="5a3e9-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="5a3e9-134">Response</span></span>
<span data-ttu-id="5a3e9-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="5a3e9-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 249

{
  "value": [
    {
      "@odata.type": "microsoft.graph.managedAppDiagnosticStatus",
      "validationName": "Validation Name value",
      "state": "State value",
      "mitigationInstruction": "Mitigation Instruction value"
    }
  ]
}
```



