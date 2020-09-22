---
title: действие Енаблеунлиценседадминстраторс
description: После включения пользователи, которым назначена роль "Администраторы" через членство в назначениях ролей, больше не требуют назначенной лицензии Intune. У вас может быть до 350 нелицензированных нелицензированных участников для каждой группы безопасности AAD в назначении ролей, но для одной роли можно назначить несколько групп безопасности AAD, если вам требуется поддержка более 350 нелицензированных администраторов. Лицензированные администраторы продолжат действовать без ограничений, так как в этом случае применяются эти транзитивные членства, и они не подчиняются ограничению члена 350.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: e6179929eec88b79a44b09c46dcd0049d7716c3b
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "47995781"
---
# <a name="enableunlicensedadminstrators-action"></a><span data-ttu-id="279f8-105">действие Енаблеунлиценседадминстраторс</span><span class="sxs-lookup"><span data-stu-id="279f8-105">enableUnlicensedAdminstrators action</span></span>

<span data-ttu-id="279f8-106">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="279f8-106">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="279f8-107">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="279f8-107">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="279f8-108">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="279f8-108">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="279f8-109">После включения пользователи, которым назначена роль "Администраторы" через членство в назначениях ролей, больше не требуют назначенной лицензии Intune.</span><span class="sxs-lookup"><span data-stu-id="279f8-109">Upon enabling, users assigned as administrators via Role Assignment Memberships will no longer require an assigned Intune license.</span></span> <span data-ttu-id="279f8-110">У вас может быть до 350 нелицензированных нелицензированных участников для каждой группы безопасности AAD в назначении ролей, но для одной роли можно назначить несколько групп безопасности AAD, если вам требуется поддержка более 350 нелицензированных администраторов.</span><span class="sxs-lookup"><span data-stu-id="279f8-110">You are limited to 350 unlicensed direct members for each AAD security group in a role assignment, but you can assign multiple AAD security groups to a role if you need to support more than 350 unlicensed administrators.</span></span> <span data-ttu-id="279f8-111">Лицензированные администраторы продолжат действовать без ограничений, так как в этом случае применяются эти транзитивные членства, и они не подчиняются ограничению члена 350.</span><span class="sxs-lookup"><span data-stu-id="279f8-111">Licensed administrators will continue to function as-is in that transitive memberships apply and are not subject to the 350 member limit.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="279f8-112">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="279f8-112">Prerequisites</span></span>
<span data-ttu-id="279f8-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="279f8-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="279f8-115">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="279f8-115">Permission type</span></span>|<span data-ttu-id="279f8-116">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="279f8-116">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="279f8-117">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="279f8-117">Delegated (work or school account)</span></span>|<span data-ttu-id="279f8-118">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="279f8-118">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="279f8-119">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="279f8-119">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="279f8-120">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="279f8-120">Not supported.</span></span>|
|<span data-ttu-id="279f8-121">Для приложений</span><span class="sxs-lookup"><span data-stu-id="279f8-121">Application</span></span>|<span data-ttu-id="279f8-122">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="279f8-122">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="279f8-123">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="279f8-123">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/enableUnlicensedAdminstrators
```

## <a name="request-headers"></a><span data-ttu-id="279f8-124">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="279f8-124">Request headers</span></span>
|<span data-ttu-id="279f8-125">Заголовок</span><span class="sxs-lookup"><span data-stu-id="279f8-125">Header</span></span>|<span data-ttu-id="279f8-126">Значение</span><span class="sxs-lookup"><span data-stu-id="279f8-126">Value</span></span>|
|:---|:---|
|<span data-ttu-id="279f8-127">Authorization</span><span class="sxs-lookup"><span data-stu-id="279f8-127">Authorization</span></span>|<span data-ttu-id="279f8-128">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="279f8-128">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="279f8-129">Accept</span><span class="sxs-lookup"><span data-stu-id="279f8-129">Accept</span></span>|<span data-ttu-id="279f8-130">application/json</span><span class="sxs-lookup"><span data-stu-id="279f8-130">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="279f8-131">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="279f8-131">Request body</span></span>
<span data-ttu-id="279f8-132">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="279f8-132">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="279f8-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="279f8-133">Response</span></span>
<span data-ttu-id="279f8-134">В случае успешного выполнения это действие возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="279f8-134">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="279f8-135">Пример</span><span class="sxs-lookup"><span data-stu-id="279f8-135">Example</span></span>

### <a name="request"></a><span data-ttu-id="279f8-136">Запрос</span><span class="sxs-lookup"><span data-stu-id="279f8-136">Request</span></span>
<span data-ttu-id="279f8-137">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="279f8-137">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/enableUnlicensedAdminstrators
```

### <a name="response"></a><span data-ttu-id="279f8-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="279f8-138">Response</span></span>
<span data-ttu-id="279f8-p104">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="279f8-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```






