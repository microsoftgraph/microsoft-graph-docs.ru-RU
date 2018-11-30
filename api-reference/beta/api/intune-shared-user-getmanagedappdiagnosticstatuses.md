---
title: Функция getManagedAppDiagnosticStatuses
description: Получает состояние диагностической проверки для определенного пользователя.
ms.openlocfilehash: bbbb399ef26c38972f989c2e1129fe61baffa0fa
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27081330"
---
# <a name="getmanagedappdiagnosticstatuses-function"></a><span data-ttu-id="2175a-103">Функция getManagedAppDiagnosticStatuses</span><span class="sxs-lookup"><span data-stu-id="2175a-103">getManagedAppDiagnosticStatuses function</span></span>

> <span data-ttu-id="2175a-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="2175a-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="2175a-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2175a-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="2175a-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="2175a-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="2175a-107">Получает состояние диагностической проверки для определенного пользователя.</span><span class="sxs-lookup"><span data-stu-id="2175a-107">Gets diagnostics validation status for a given user.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="2175a-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="2175a-108">Prerequisites</span></span>
<span data-ttu-id="2175a-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2175a-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2175a-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="2175a-111">Permission type</span></span>|<span data-ttu-id="2175a-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="2175a-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2175a-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="2175a-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="2175a-114">&nbsp;&nbsp; **MAM**</span><span class="sxs-lookup"><span data-stu-id="2175a-114">&nbsp; &nbsp; **MAM**</span></span> | <span data-ttu-id="2175a-115">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="2175a-115">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="2175a-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="2175a-116">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2175a-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2175a-117">Not supported.</span></span>|
|<span data-ttu-id="2175a-118">Для приложений</span><span class="sxs-lookup"><span data-stu-id="2175a-118">Application</span></span>|<span data-ttu-id="2175a-119">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2175a-119">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="2175a-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="2175a-120">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /users/{usersId}/getManagedAppDiagnosticStatuses
```

## <a name="request-headers"></a><span data-ttu-id="2175a-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="2175a-121">Request headers</span></span>
|<span data-ttu-id="2175a-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="2175a-122">Header</span></span>|<span data-ttu-id="2175a-123">Значение</span><span class="sxs-lookup"><span data-stu-id="2175a-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="2175a-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="2175a-124">Authorization</span></span>|<span data-ttu-id="2175a-125">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="2175a-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="2175a-126">Accept</span><span class="sxs-lookup"><span data-stu-id="2175a-126">Accept</span></span>|<span data-ttu-id="2175a-127">application/json</span><span class="sxs-lookup"><span data-stu-id="2175a-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="2175a-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="2175a-128">Request body</span></span>
<span data-ttu-id="2175a-129">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="2175a-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="2175a-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="2175a-130">Response</span></span>
<span data-ttu-id="2175a-131">При успешном выполнении эта функция возвращает код отклика `200 OK` и коллекцию [managedAppDiagnosticStatus](../resources/intune-mam-managedappdiagnosticstatus.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="2175a-131">If successful, this function returns a `200 OK` response code and a [managedAppDiagnosticStatus](../resources/intune-mam-managedappdiagnosticstatus.md) collection in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2175a-132">Пример</span><span class="sxs-lookup"><span data-stu-id="2175a-132">Example</span></span>
### <a name="request"></a><span data-ttu-id="2175a-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="2175a-133">Request</span></span>
<span data-ttu-id="2175a-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="2175a-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/users/{usersId}/getManagedAppDiagnosticStatuses
```

### <a name="response"></a><span data-ttu-id="2175a-135">Ответ</span><span class="sxs-lookup"><span data-stu-id="2175a-135">Response</span></span>
<span data-ttu-id="2175a-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
</span><span class="sxs-lookup"><span data-stu-id="2175a-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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






