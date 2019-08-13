---
title: Удаление Граупполиципресентатионвалуемултитекст
description: Удаляет объект Граупполиципресентатионвалуемултитекст.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: c21f870dedee5dd2a5650cc95ddc6bd91d938b20
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/13/2019
ms.locfileid: "36354473"
---
# <a name="delete-grouppolicypresentationvaluemultitext"></a><span data-ttu-id="350ec-103">Удаление Граупполиципресентатионвалуемултитекст</span><span class="sxs-lookup"><span data-stu-id="350ec-103">Delete groupPolicyPresentationValueMultiText</span></span>

> <span data-ttu-id="350ec-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="350ec-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="350ec-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="350ec-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="350ec-106">Удаляет объект [граупполиципресентатионвалуемултитекст](../resources/intune-grouppolicy-grouppolicypresentationvaluemultitext.md).</span><span class="sxs-lookup"><span data-stu-id="350ec-106">Deletes a [groupPolicyPresentationValueMultiText](../resources/intune-grouppolicy-grouppolicypresentationvaluemultitext.md).</span></span>

## <a name="prerequisites"></a><span data-ttu-id="350ec-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="350ec-107">Prerequisites</span></span>
<span data-ttu-id="350ec-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="350ec-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="350ec-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="350ec-110">Permission type</span></span>|<span data-ttu-id="350ec-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="350ec-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="350ec-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="350ec-112">Delegated (work or school account)</span></span>|<span data-ttu-id="350ec-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="350ec-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="350ec-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="350ec-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="350ec-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="350ec-115">Not supported.</span></span>|
|<span data-ttu-id="350ec-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="350ec-116">Application</span></span>|<span data-ttu-id="350ec-117">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="350ec-117">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="350ec-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="350ec-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}
```

## <a name="request-headers"></a><span data-ttu-id="350ec-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="350ec-119">Request headers</span></span>
|<span data-ttu-id="350ec-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="350ec-120">Header</span></span>|<span data-ttu-id="350ec-121">Значение</span><span class="sxs-lookup"><span data-stu-id="350ec-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="350ec-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="350ec-122">Authorization</span></span>|<span data-ttu-id="350ec-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="350ec-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="350ec-124">Accept</span><span class="sxs-lookup"><span data-stu-id="350ec-124">Accept</span></span>|<span data-ttu-id="350ec-125">application/json</span><span class="sxs-lookup"><span data-stu-id="350ec-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="350ec-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="350ec-126">Request body</span></span>
<span data-ttu-id="350ec-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="350ec-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="350ec-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="350ec-128">Response</span></span>
<span data-ttu-id="350ec-129">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="350ec-129">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="350ec-130">Пример</span><span class="sxs-lookup"><span data-stu-id="350ec-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="350ec-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="350ec-131">Request</span></span>
<span data-ttu-id="350ec-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="350ec-132">Here is an example of the request.</span></span>
``` http
DELETE https://graph.microsoft.com/beta/deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}
```

### <a name="response"></a><span data-ttu-id="350ec-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="350ec-133">Response</span></span>
<span data-ttu-id="350ec-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="350ec-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```






