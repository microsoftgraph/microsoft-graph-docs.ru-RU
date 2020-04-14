---
title: Функция getManagedAppDiagnosticStatuses
description: Получает состояние диагностической проверки для определенного пользователя.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 0c3930dd8e70deb2324fbb6e95694cf0be9a05c2
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43447509"
---
# <a name="getmanagedappdiagnosticstatuses-function"></a><span data-ttu-id="aa24f-103">Функция getManagedAppDiagnosticStatuses</span><span class="sxs-lookup"><span data-stu-id="aa24f-103">getManagedAppDiagnosticStatuses function</span></span>

<span data-ttu-id="aa24f-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="aa24f-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="aa24f-105">**Важно!** API в версии/Beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="aa24f-105">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="aa24f-106">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="aa24f-106">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="aa24f-107">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="aa24f-107">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="aa24f-108">Получает состояние диагностической проверки для определенного пользователя.</span><span class="sxs-lookup"><span data-stu-id="aa24f-108">Gets diagnostics validation status for a given user.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="aa24f-109">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="aa24f-109">Prerequisites</span></span>
<span data-ttu-id="aa24f-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="aa24f-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="aa24f-112">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="aa24f-112">Permission type</span></span>|<span data-ttu-id="aa24f-113">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="aa24f-113">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="aa24f-114">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="aa24f-114">Delegated (work or school account)</span></span>||
| <span data-ttu-id="aa24f-115">&nbsp;&nbsp; **MAM**</span><span class="sxs-lookup"><span data-stu-id="aa24f-115">&nbsp; &nbsp; **MAM**</span></span> | <span data-ttu-id="aa24f-116">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="aa24f-116">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="aa24f-117">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="aa24f-117">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="aa24f-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="aa24f-118">Not supported.</span></span>|
|<span data-ttu-id="aa24f-119">Для приложений</span><span class="sxs-lookup"><span data-stu-id="aa24f-119">Application</span></span>||
| <span data-ttu-id="aa24f-120">&nbsp;&nbsp; **MAM**</span><span class="sxs-lookup"><span data-stu-id="aa24f-120">&nbsp; &nbsp; **MAM**</span></span> | <span data-ttu-id="aa24f-121">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="aa24f-121">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="aa24f-122">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="aa24f-122">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /users/{usersId}/getManagedAppDiagnosticStatuses
```

## <a name="request-headers"></a><span data-ttu-id="aa24f-123">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="aa24f-123">Request headers</span></span>
|<span data-ttu-id="aa24f-124">Заголовок</span><span class="sxs-lookup"><span data-stu-id="aa24f-124">Header</span></span>|<span data-ttu-id="aa24f-125">Значение</span><span class="sxs-lookup"><span data-stu-id="aa24f-125">Value</span></span>|
|:---|:---|
|<span data-ttu-id="aa24f-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="aa24f-126">Authorization</span></span>|<span data-ttu-id="aa24f-127">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="aa24f-127">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="aa24f-128">Accept</span><span class="sxs-lookup"><span data-stu-id="aa24f-128">Accept</span></span>|<span data-ttu-id="aa24f-129">application/json</span><span class="sxs-lookup"><span data-stu-id="aa24f-129">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="aa24f-130">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="aa24f-130">Request body</span></span>
<span data-ttu-id="aa24f-131">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="aa24f-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="aa24f-132">Ответ</span><span class="sxs-lookup"><span data-stu-id="aa24f-132">Response</span></span>
<span data-ttu-id="aa24f-133">При успешном выполнении эта функция возвращает код отклика `200 OK` и коллекцию [managedAppDiagnosticStatus](../resources/intune-mam-managedappdiagnosticstatus.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="aa24f-133">If successful, this function returns a `200 OK` response code and a [managedAppDiagnosticStatus](../resources/intune-mam-managedappdiagnosticstatus.md) collection in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="aa24f-134">Пример</span><span class="sxs-lookup"><span data-stu-id="aa24f-134">Example</span></span>
### <a name="request"></a><span data-ttu-id="aa24f-135">Запрос</span><span class="sxs-lookup"><span data-stu-id="aa24f-135">Request</span></span>
<span data-ttu-id="aa24f-136">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="aa24f-136">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/users/{usersId}/getManagedAppDiagnosticStatuses
```

### <a name="response"></a><span data-ttu-id="aa24f-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="aa24f-137">Response</span></span>
<span data-ttu-id="aa24f-p103">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="aa24f-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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












