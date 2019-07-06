---
title: Удаление Граупполиципресентатионлистбокс
description: Удаляет объект Граупполиципресентатионлистбокс.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 0f98dc71eeb618188a4c799059879506e4c660e8
ms.sourcegitcommit: 705b32b9a64516d8138fab34c173b7df4f78a6ad
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/05/2019
ms.locfileid: "35576454"
---
# <a name="delete-grouppolicypresentationlistbox"></a><span data-ttu-id="ef82f-103">Удаление Граупполиципресентатионлистбокс</span><span class="sxs-lookup"><span data-stu-id="ef82f-103">Delete groupPolicyPresentationListBox</span></span>

> <span data-ttu-id="ef82f-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ef82f-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ef82f-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="ef82f-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ef82f-106">Удаляет объект [граупполиципресентатионлистбокс](../resources/intune-grouppolicy-grouppolicypresentationlistbox.md).</span><span class="sxs-lookup"><span data-stu-id="ef82f-106">Deletes a [groupPolicyPresentationListBox](../resources/intune-grouppolicy-grouppolicypresentationlistbox.md).</span></span>

## <a name="prerequisites"></a><span data-ttu-id="ef82f-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="ef82f-107">Prerequisites</span></span>
<span data-ttu-id="ef82f-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ef82f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ef82f-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ef82f-110">Permission type</span></span>|<span data-ttu-id="ef82f-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="ef82f-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ef82f-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ef82f-112">Delegated (work or school account)</span></span>|<span data-ttu-id="ef82f-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ef82f-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="ef82f-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ef82f-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ef82f-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ef82f-115">Not supported.</span></span>|
|<span data-ttu-id="ef82f-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="ef82f-116">Application</span></span>|<span data-ttu-id="ef82f-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ef82f-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="ef82f-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ef82f-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation
DELETE /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation/definition/presentations/{groupPolicyPresentationId}
```

## <a name="request-headers"></a><span data-ttu-id="ef82f-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="ef82f-119">Request headers</span></span>
|<span data-ttu-id="ef82f-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="ef82f-120">Header</span></span>|<span data-ttu-id="ef82f-121">Значение</span><span class="sxs-lookup"><span data-stu-id="ef82f-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ef82f-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="ef82f-122">Authorization</span></span>|<span data-ttu-id="ef82f-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="ef82f-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ef82f-124">Accept</span><span class="sxs-lookup"><span data-stu-id="ef82f-124">Accept</span></span>|<span data-ttu-id="ef82f-125">application/json</span><span class="sxs-lookup"><span data-stu-id="ef82f-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ef82f-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="ef82f-126">Request body</span></span>
<span data-ttu-id="ef82f-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="ef82f-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ef82f-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="ef82f-128">Response</span></span>
<span data-ttu-id="ef82f-129">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="ef82f-129">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="ef82f-130">Пример</span><span class="sxs-lookup"><span data-stu-id="ef82f-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="ef82f-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="ef82f-131">Request</span></span>
<span data-ttu-id="ef82f-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="ef82f-132">Here is an example of the request.</span></span>
``` http
DELETE https://graph.microsoft.com/beta/deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation
```

### <a name="response"></a><span data-ttu-id="ef82f-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="ef82f-133">Response</span></span>
<span data-ttu-id="ef82f-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="ef82f-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```



