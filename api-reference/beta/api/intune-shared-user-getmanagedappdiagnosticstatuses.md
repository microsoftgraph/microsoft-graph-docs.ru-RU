---
title: Функция getManagedAppDiagnosticStatuses
description: Получает состояние диагностической проверки для определенного пользователя.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 4b24f6d647612dfe142cd6fad3709c8b2186c3b4
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/22/2020
ms.locfileid: "48698038"
---
# <a name="getmanagedappdiagnosticstatuses-function"></a><span data-ttu-id="7aaa2-103">Функция getManagedAppDiagnosticStatuses</span><span class="sxs-lookup"><span data-stu-id="7aaa2-103">getManagedAppDiagnosticStatuses function</span></span>

<span data-ttu-id="7aaa2-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7aaa2-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="7aaa2-105">**Важно!** API в версии/Beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="7aaa2-105">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="7aaa2-106">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7aaa2-106">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="7aaa2-107">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="7aaa2-107">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7aaa2-108">Получает состояние диагностической проверки для определенного пользователя.</span><span class="sxs-lookup"><span data-stu-id="7aaa2-108">Gets diagnostics validation status for a given user.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="7aaa2-109">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="7aaa2-109">Prerequisites</span></span>
<span data-ttu-id="7aaa2-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7aaa2-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7aaa2-112">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="7aaa2-112">Permission type</span></span>|<span data-ttu-id="7aaa2-113">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="7aaa2-113">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="7aaa2-114">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="7aaa2-114">Delegated (work or school account)</span></span>||
| <span data-ttu-id="7aaa2-115">&nbsp;&nbsp; **MAM**</span><span class="sxs-lookup"><span data-stu-id="7aaa2-115">&nbsp; &nbsp; **MAM**</span></span> | <span data-ttu-id="7aaa2-116">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="7aaa2-116">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="7aaa2-117">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="7aaa2-117">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7aaa2-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7aaa2-118">Not supported.</span></span>|
|<span data-ttu-id="7aaa2-119">Для приложений</span><span class="sxs-lookup"><span data-stu-id="7aaa2-119">Application</span></span>||
| <span data-ttu-id="7aaa2-120">&nbsp;&nbsp; **MAM**</span><span class="sxs-lookup"><span data-stu-id="7aaa2-120">&nbsp; &nbsp; **MAM**</span></span> | <span data-ttu-id="7aaa2-121">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="7aaa2-121">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="7aaa2-122">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="7aaa2-122">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /users/{usersId}/getManagedAppDiagnosticStatuses
```

## <a name="request-headers"></a><span data-ttu-id="7aaa2-123">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="7aaa2-123">Request headers</span></span>
|<span data-ttu-id="7aaa2-124">Заголовок</span><span class="sxs-lookup"><span data-stu-id="7aaa2-124">Header</span></span>|<span data-ttu-id="7aaa2-125">Значение</span><span class="sxs-lookup"><span data-stu-id="7aaa2-125">Value</span></span>|
|:---|:---|
|<span data-ttu-id="7aaa2-126">Авторизация</span><span class="sxs-lookup"><span data-stu-id="7aaa2-126">Authorization</span></span>|<span data-ttu-id="7aaa2-127">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="7aaa2-127">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="7aaa2-128">Accept</span><span class="sxs-lookup"><span data-stu-id="7aaa2-128">Accept</span></span>|<span data-ttu-id="7aaa2-129">application/json</span><span class="sxs-lookup"><span data-stu-id="7aaa2-129">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="7aaa2-130">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="7aaa2-130">Request body</span></span>
<span data-ttu-id="7aaa2-131">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="7aaa2-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="7aaa2-132">Ответ</span><span class="sxs-lookup"><span data-stu-id="7aaa2-132">Response</span></span>
<span data-ttu-id="7aaa2-133">При успешном выполнении эта функция возвращает код отклика `200 OK` и коллекцию [managedAppDiagnosticStatus](../resources/intune-mam-managedappdiagnosticstatus.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="7aaa2-133">If successful, this function returns a `200 OK` response code and a [managedAppDiagnosticStatus](../resources/intune-mam-managedappdiagnosticstatus.md) collection in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7aaa2-134">Пример</span><span class="sxs-lookup"><span data-stu-id="7aaa2-134">Example</span></span>
### <a name="request"></a><span data-ttu-id="7aaa2-135">Запрос</span><span class="sxs-lookup"><span data-stu-id="7aaa2-135">Request</span></span>
<span data-ttu-id="7aaa2-136">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="7aaa2-136">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/users/{usersId}/getManagedAppDiagnosticStatuses
```

### <a name="response"></a><span data-ttu-id="7aaa2-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="7aaa2-137">Response</span></span>
<span data-ttu-id="7aaa2-p103">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="7aaa2-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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














