---
title: Функция getManagedAppDiagnosticStatuses
description: Получает состояние диагностической проверки для определенного пользователя.
author: davidmu1
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 9d08785b8eff6d8233476132d21934336eadd076
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42511987"
---
# <a name="getmanagedappdiagnosticstatuses-function"></a><span data-ttu-id="40ebd-103">Функция getManagedAppDiagnosticStatuses</span><span class="sxs-lookup"><span data-stu-id="40ebd-103">getManagedAppDiagnosticStatuses function</span></span>

<span data-ttu-id="40ebd-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="40ebd-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="40ebd-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="40ebd-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="40ebd-106">Получает состояние диагностической проверки для определенного пользователя.</span><span class="sxs-lookup"><span data-stu-id="40ebd-106">Gets diagnostics validation status for a given user.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="40ebd-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="40ebd-107">Prerequisites</span></span>
<span data-ttu-id="40ebd-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="40ebd-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="40ebd-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="40ebd-110">Permission type</span></span>|<span data-ttu-id="40ebd-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="40ebd-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="40ebd-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="40ebd-112">Delegated (work or school account)</span></span>| <span data-ttu-id="40ebd-113">_зависит от контекста_</span><span class="sxs-lookup"><span data-stu-id="40ebd-113">_varies by context_</span></span>|
| <span data-ttu-id="40ebd-114">&nbsp;&nbsp; MAM</span><span class="sxs-lookup"><span data-stu-id="40ebd-114">&nbsp; &nbsp; MAM</span></span> | <span data-ttu-id="40ebd-115">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="40ebd-115">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span> |
|<span data-ttu-id="40ebd-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="40ebd-116">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="40ebd-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="40ebd-117">Not supported.</span></span>|
|<span data-ttu-id="40ebd-118">Для приложений</span><span class="sxs-lookup"><span data-stu-id="40ebd-118">Application</span></span>|<span data-ttu-id="40ebd-119">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="40ebd-119">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="40ebd-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="40ebd-120">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /users/{usersId}/getManagedAppDiagnosticStatuses
```

## <a name="request-headers"></a><span data-ttu-id="40ebd-121">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="40ebd-121">Request headers</span></span>
|<span data-ttu-id="40ebd-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="40ebd-122">Header</span></span>|<span data-ttu-id="40ebd-123">Значение</span><span class="sxs-lookup"><span data-stu-id="40ebd-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="40ebd-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="40ebd-124">Authorization</span></span>|<span data-ttu-id="40ebd-125">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="40ebd-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="40ebd-126">Accept</span><span class="sxs-lookup"><span data-stu-id="40ebd-126">Accept</span></span>|<span data-ttu-id="40ebd-127">application/json</span><span class="sxs-lookup"><span data-stu-id="40ebd-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="40ebd-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="40ebd-128">Request body</span></span>
<span data-ttu-id="40ebd-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="40ebd-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="40ebd-130">Ответ</span><span class="sxs-lookup"><span data-stu-id="40ebd-130">Response</span></span>
<span data-ttu-id="40ebd-131">При успешном выполнении эта функция возвращает код отклика `200 OK` и коллекцию [managedAppDiagnosticStatus](../resources/intune-mam-managedappdiagnosticstatus.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="40ebd-131">If successful, this function returns a `200 OK` response code and a [managedAppDiagnosticStatus](../resources/intune-mam-managedappdiagnosticstatus.md) collection in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="40ebd-132">Пример</span><span class="sxs-lookup"><span data-stu-id="40ebd-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="40ebd-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="40ebd-133">Request</span></span>
<span data-ttu-id="40ebd-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="40ebd-134">Here is an example of the request.</span></span>

``` http
GET https://graph.microsoft.com/v1.0/users/{usersId}/getManagedAppDiagnosticStatuses
```

### <a name="response"></a><span data-ttu-id="40ebd-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="40ebd-135">Response</span></span>
<span data-ttu-id="40ebd-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="40ebd-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

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




