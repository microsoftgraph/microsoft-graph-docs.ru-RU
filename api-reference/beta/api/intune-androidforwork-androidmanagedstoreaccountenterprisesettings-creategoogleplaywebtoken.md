---
title: Действие createGooglePlayWebToken
description: Создает веб-маркер, используемый в встраивомом компоненте.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 6cc813873b865eb03c76a68f40141b3b42bac044
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51141199"
---
# <a name="creategoogleplaywebtoken-action"></a><span data-ttu-id="0b31b-103">Действие createGooglePlayWebToken</span><span class="sxs-lookup"><span data-stu-id="0b31b-103">createGooglePlayWebToken action</span></span>

<span data-ttu-id="0b31b-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0b31b-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="0b31b-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0b31b-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="0b31b-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="0b31b-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0b31b-107">Создает веб-маркер, используемый в встраивомом компоненте.</span><span class="sxs-lookup"><span data-stu-id="0b31b-107">Generates a web token that is used in an embeddable component.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="0b31b-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="0b31b-108">Prerequisites</span></span>
<span data-ttu-id="0b31b-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0b31b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0b31b-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="0b31b-111">Permission type</span></span>|<span data-ttu-id="0b31b-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="0b31b-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0b31b-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="0b31b-113">Delegated (work or school account)</span></span>|<span data-ttu-id="0b31b-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0b31b-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="0b31b-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="0b31b-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0b31b-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0b31b-116">Not supported.</span></span>|
|<span data-ttu-id="0b31b-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="0b31b-117">Application</span></span>|<span data-ttu-id="0b31b-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0b31b-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="0b31b-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="0b31b-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/androidManagedStoreAccountEnterpriseSettings/createGooglePlayWebToken
```

## <a name="request-headers"></a><span data-ttu-id="0b31b-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="0b31b-120">Request headers</span></span>
|<span data-ttu-id="0b31b-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="0b31b-121">Header</span></span>|<span data-ttu-id="0b31b-122">Значение</span><span class="sxs-lookup"><span data-stu-id="0b31b-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="0b31b-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="0b31b-123">Authorization</span></span>|<span data-ttu-id="0b31b-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="0b31b-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="0b31b-125">Accept</span><span class="sxs-lookup"><span data-stu-id="0b31b-125">Accept</span></span>|<span data-ttu-id="0b31b-126">application/json</span><span class="sxs-lookup"><span data-stu-id="0b31b-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="0b31b-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="0b31b-127">Request body</span></span>
<span data-ttu-id="0b31b-128">В тело запроса добавьте параметры в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="0b31b-128">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="0b31b-129">В приведенной ниже таблице указаны параметры, которые можно использовать с этим действием.</span><span class="sxs-lookup"><span data-stu-id="0b31b-129">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="0b31b-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="0b31b-130">Property</span></span>|<span data-ttu-id="0b31b-131">Тип</span><span class="sxs-lookup"><span data-stu-id="0b31b-131">Type</span></span>|<span data-ttu-id="0b31b-132">Описание</span><span class="sxs-lookup"><span data-stu-id="0b31b-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0b31b-133">parentUri</span><span class="sxs-lookup"><span data-stu-id="0b31b-133">parentUri</span></span>|<span data-ttu-id="0b31b-134">Строка</span><span class="sxs-lookup"><span data-stu-id="0b31b-134">String</span></span>|<span data-ttu-id="0b31b-135">Путь https страницы, на которая размещен компонент.</span><span class="sxs-lookup"><span data-stu-id="0b31b-135">The https path of the page hosting the component.</span></span>|



## <a name="response"></a><span data-ttu-id="0b31b-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="0b31b-136">Response</span></span>
<span data-ttu-id="0b31b-137">При успешном выполнении это действие возвращает код отклика `200 OK` и объект String в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="0b31b-137">If successful, this action returns a `200 OK` response code and a String in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0b31b-138">Пример</span><span class="sxs-lookup"><span data-stu-id="0b31b-138">Example</span></span>

### <a name="request"></a><span data-ttu-id="0b31b-139">Запрос</span><span class="sxs-lookup"><span data-stu-id="0b31b-139">Request</span></span>
<span data-ttu-id="0b31b-140">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="0b31b-140">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/androidManagedStoreAccountEnterpriseSettings/createGooglePlayWebToken

Content-type: application/json
Content-length: 39

{
  "parentUri": "Parent Uri value"
}
```

### <a name="response"></a><span data-ttu-id="0b31b-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="0b31b-141">Response</span></span>
<span data-ttu-id="0b31b-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="0b31b-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 53

{
  "value": "Create Google Play Web Token value"
}
```




