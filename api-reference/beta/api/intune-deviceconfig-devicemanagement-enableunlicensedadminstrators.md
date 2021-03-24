---
title: enableUnlicensedAdminstrators action
description: После включения пользователям, назначенным администраторами с помощью членов назначения ролей, больше не потребуется назначенная лицензия Intune. Для каждой группы безопасности AAD в назначении ролей может быть ограничено 350 нелицензионных прямых членов, но при необходимости для поддержки более 350 нелицензионных администраторов можно назначить несколько групп безопасности AAD. Лицензированные администраторы будут продолжать функционировать как есть в том, что транзитные членства применяются и не подлежат ограничению в 350 членов.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 149c14aab5672939174799791f6a4e0af970419d
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51128028"
---
# <a name="enableunlicensedadminstrators-action"></a><span data-ttu-id="0c0e1-105">enableUnlicensedAdminstrators action</span><span class="sxs-lookup"><span data-stu-id="0c0e1-105">enableUnlicensedAdminstrators action</span></span>

<span data-ttu-id="0c0e1-106">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0c0e1-106">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="0c0e1-107">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0c0e1-107">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="0c0e1-108">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="0c0e1-108">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0c0e1-109">После включения пользователям, назначенным администраторами с помощью членов назначения ролей, больше не потребуется назначенная лицензия Intune.</span><span class="sxs-lookup"><span data-stu-id="0c0e1-109">Upon enabling, users assigned as administrators via Role Assignment Memberships will no longer require an assigned Intune license.</span></span> <span data-ttu-id="0c0e1-110">Для каждой группы безопасности AAD в назначении ролей может быть ограничено 350 нелицензионных прямых членов, но при необходимости для поддержки более 350 нелицензионных администраторов можно назначить несколько групп безопасности AAD.</span><span class="sxs-lookup"><span data-stu-id="0c0e1-110">You are limited to 350 unlicensed direct members for each AAD security group in a role assignment, but you can assign multiple AAD security groups to a role if you need to support more than 350 unlicensed administrators.</span></span> <span data-ttu-id="0c0e1-111">Лицензированные администраторы будут продолжать функционировать как есть в том, что транзитные членства применяются и не подлежат ограничению в 350 членов.</span><span class="sxs-lookup"><span data-stu-id="0c0e1-111">Licensed administrators will continue to function as-is in that transitive memberships apply and are not subject to the 350 member limit.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="0c0e1-112">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="0c0e1-112">Prerequisites</span></span>
<span data-ttu-id="0c0e1-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0c0e1-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0c0e1-115">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="0c0e1-115">Permission type</span></span>|<span data-ttu-id="0c0e1-116">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="0c0e1-116">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0c0e1-117">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="0c0e1-117">Delegated (work or school account)</span></span>|<span data-ttu-id="0c0e1-118">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0c0e1-118">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="0c0e1-119">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="0c0e1-119">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0c0e1-120">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0c0e1-120">Not supported.</span></span>|
|<span data-ttu-id="0c0e1-121">Приложение</span><span class="sxs-lookup"><span data-stu-id="0c0e1-121">Application</span></span>|<span data-ttu-id="0c0e1-122">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0c0e1-122">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="0c0e1-123">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="0c0e1-123">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/enableUnlicensedAdminstrators
```

## <a name="request-headers"></a><span data-ttu-id="0c0e1-124">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="0c0e1-124">Request headers</span></span>
|<span data-ttu-id="0c0e1-125">Заголовок</span><span class="sxs-lookup"><span data-stu-id="0c0e1-125">Header</span></span>|<span data-ttu-id="0c0e1-126">Значение</span><span class="sxs-lookup"><span data-stu-id="0c0e1-126">Value</span></span>|
|:---|:---|
|<span data-ttu-id="0c0e1-127">Authorization</span><span class="sxs-lookup"><span data-stu-id="0c0e1-127">Authorization</span></span>|<span data-ttu-id="0c0e1-128">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="0c0e1-128">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="0c0e1-129">Accept</span><span class="sxs-lookup"><span data-stu-id="0c0e1-129">Accept</span></span>|<span data-ttu-id="0c0e1-130">application/json</span><span class="sxs-lookup"><span data-stu-id="0c0e1-130">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="0c0e1-131">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="0c0e1-131">Request body</span></span>
<span data-ttu-id="0c0e1-132">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="0c0e1-132">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="0c0e1-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="0c0e1-133">Response</span></span>
<span data-ttu-id="0c0e1-134">В случае успешного выполнения это действие возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="0c0e1-134">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="0c0e1-135">Пример</span><span class="sxs-lookup"><span data-stu-id="0c0e1-135">Example</span></span>

### <a name="request"></a><span data-ttu-id="0c0e1-136">Запрос</span><span class="sxs-lookup"><span data-stu-id="0c0e1-136">Request</span></span>
<span data-ttu-id="0c0e1-137">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="0c0e1-137">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/enableUnlicensedAdminstrators
```

### <a name="response"></a><span data-ttu-id="0c0e1-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="0c0e1-138">Response</span></span>
<span data-ttu-id="0c0e1-p104">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="0c0e1-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```




