---
title: Удаление ГраупполиципресентатиондеЦималтекстбокс
description: Удаляет объект ГраупполиципресентатиондеЦималтекстбокс.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 58a5f5bc5237eb352805366ca382b4ac47d591b5
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43424568"
---
# <a name="delete-grouppolicypresentationdecimaltextbox"></a><span data-ttu-id="88052-103">Удаление ГраупполиципресентатиондеЦималтекстбокс</span><span class="sxs-lookup"><span data-stu-id="88052-103">Delete groupPolicyPresentationDecimalTextBox</span></span>

<span data-ttu-id="88052-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="88052-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="88052-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="88052-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="88052-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="88052-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="88052-107">Удаляет объект [граупполиципресентатиондеЦималтекстбокс](../resources/intune-grouppolicy-grouppolicypresentationdecimaltextbox.md).</span><span class="sxs-lookup"><span data-stu-id="88052-107">Deletes a [groupPolicyPresentationDecimalTextBox](../resources/intune-grouppolicy-grouppolicypresentationdecimaltextbox.md).</span></span>

## <a name="prerequisites"></a><span data-ttu-id="88052-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="88052-108">Prerequisites</span></span>
<span data-ttu-id="88052-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="88052-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="88052-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="88052-111">Permission type</span></span>|<span data-ttu-id="88052-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="88052-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="88052-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="88052-113">Delegated (work or school account)</span></span>|<span data-ttu-id="88052-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="88052-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="88052-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="88052-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="88052-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="88052-116">Not supported.</span></span>|
|<span data-ttu-id="88052-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="88052-117">Application</span></span>|<span data-ttu-id="88052-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="88052-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="88052-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="88052-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation
DELETE /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation/definition/presentations/{groupPolicyPresentationId}
```

## <a name="request-headers"></a><span data-ttu-id="88052-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="88052-120">Request headers</span></span>
|<span data-ttu-id="88052-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="88052-121">Header</span></span>|<span data-ttu-id="88052-122">Значение</span><span class="sxs-lookup"><span data-stu-id="88052-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="88052-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="88052-123">Authorization</span></span>|<span data-ttu-id="88052-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="88052-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="88052-125">Accept</span><span class="sxs-lookup"><span data-stu-id="88052-125">Accept</span></span>|<span data-ttu-id="88052-126">application/json</span><span class="sxs-lookup"><span data-stu-id="88052-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="88052-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="88052-127">Request body</span></span>
<span data-ttu-id="88052-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="88052-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="88052-129">Ответ</span><span class="sxs-lookup"><span data-stu-id="88052-129">Response</span></span>
<span data-ttu-id="88052-130">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="88052-130">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="88052-131">Пример</span><span class="sxs-lookup"><span data-stu-id="88052-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="88052-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="88052-132">Request</span></span>
<span data-ttu-id="88052-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="88052-133">Here is an example of the request.</span></span>
``` http
DELETE https://graph.microsoft.com/beta/deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation
```

### <a name="response"></a><span data-ttu-id="88052-134">Ответ</span><span class="sxs-lookup"><span data-stu-id="88052-134">Response</span></span>
<span data-ttu-id="88052-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="88052-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```



