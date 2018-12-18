---
title: Удаление androidWorkProfileGeneralDeviceConfiguration
description: Удаляет androidWorkProfileGeneralDeviceConfiguration.
author: tfitzmac
ms.openlocfilehash: 11ca11af56066d8bdd113ae4d5e55daceb843e3a
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27340749"
---
# <a name="delete-androidworkprofilegeneraldeviceconfiguration"></a><span data-ttu-id="a31cc-103">Удаление androidWorkProfileGeneralDeviceConfiguration</span><span class="sxs-lookup"><span data-stu-id="a31cc-103">Delete androidWorkProfileGeneralDeviceConfiguration</span></span>

> <span data-ttu-id="a31cc-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="a31cc-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="a31cc-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a31cc-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="a31cc-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="a31cc-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="a31cc-107">Удаляет [androidWorkProfileGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidworkprofilegeneraldeviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="a31cc-107">Deletes a [androidWorkProfileGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidworkprofilegeneraldeviceconfiguration.md).</span></span>
## <a name="prerequisites"></a><span data-ttu-id="a31cc-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="a31cc-108">Prerequisites</span></span>
<span data-ttu-id="a31cc-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a31cc-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a31cc-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="a31cc-111">Permission type</span></span>|<span data-ttu-id="a31cc-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="a31cc-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a31cc-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a31cc-113">Delegated (work or school account)</span></span>|<span data-ttu-id="a31cc-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a31cc-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="a31cc-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a31cc-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a31cc-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a31cc-116">Not supported.</span></span>|
|<span data-ttu-id="a31cc-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="a31cc-117">Application</span></span>|<span data-ttu-id="a31cc-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a31cc-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="a31cc-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a31cc-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /deviceManagement/deviceConfigurations/{deviceConfigurationId}
DELETE /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
DELETE /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="a31cc-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="a31cc-120">Request headers</span></span>
|<span data-ttu-id="a31cc-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="a31cc-121">Header</span></span>|<span data-ttu-id="a31cc-122">Значение</span><span class="sxs-lookup"><span data-stu-id="a31cc-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a31cc-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="a31cc-123">Authorization</span></span>|<span data-ttu-id="a31cc-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="a31cc-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a31cc-125">Accept</span><span class="sxs-lookup"><span data-stu-id="a31cc-125">Accept</span></span>|<span data-ttu-id="a31cc-126">application/json</span><span class="sxs-lookup"><span data-stu-id="a31cc-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a31cc-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="a31cc-127">Request body</span></span>
<span data-ttu-id="a31cc-128">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="a31cc-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a31cc-129">Ответ</span><span class="sxs-lookup"><span data-stu-id="a31cc-129">Response</span></span>
<span data-ttu-id="a31cc-130">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="a31cc-130">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="a31cc-131">Пример</span><span class="sxs-lookup"><span data-stu-id="a31cc-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="a31cc-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="a31cc-132">Request</span></span>
<span data-ttu-id="a31cc-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="a31cc-133">Here is an example of the request.</span></span>
``` http
DELETE https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

### <a name="response"></a><span data-ttu-id="a31cc-134">Ответ</span><span class="sxs-lookup"><span data-stu-id="a31cc-134">Response</span></span>
<span data-ttu-id="a31cc-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="a31cc-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```





