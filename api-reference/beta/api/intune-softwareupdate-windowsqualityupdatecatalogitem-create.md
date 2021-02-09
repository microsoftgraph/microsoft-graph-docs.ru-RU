---
title: Создание windowsQualityUpdateCatalogItem
description: Создание объекта windowsQualityUpdateCatalogItem.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: ad143f79bdabc99dadef3009bc10d55263acca1d
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/09/2021
ms.locfileid: "50160655"
---
# <a name="create-windowsqualityupdatecatalogitem"></a><span data-ttu-id="b2fbb-103">Создание windowsQualityUpdateCatalogItem</span><span class="sxs-lookup"><span data-stu-id="b2fbb-103">Create windowsQualityUpdateCatalogItem</span></span>

<span data-ttu-id="b2fbb-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b2fbb-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="b2fbb-105">**Важно!** API Microsoft Graph в бета-версии могут изменяться; использование в производственной области не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b2fbb-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b2fbb-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="b2fbb-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b2fbb-107">Создание объекта [windowsQualityUpdateCatalogItem.](../resources/intune-softwareupdate-windowsqualityupdatecatalogitem.md)</span><span class="sxs-lookup"><span data-stu-id="b2fbb-107">Create a new [windowsQualityUpdateCatalogItem](../resources/intune-softwareupdate-windowsqualityupdatecatalogitem.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="b2fbb-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="b2fbb-108">Prerequisites</span></span>
<span data-ttu-id="b2fbb-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b2fbb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b2fbb-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="b2fbb-111">Permission type</span></span>|<span data-ttu-id="b2fbb-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="b2fbb-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b2fbb-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="b2fbb-113">Delegated (work or school account)</span></span>|<span data-ttu-id="b2fbb-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b2fbb-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="b2fbb-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="b2fbb-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b2fbb-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b2fbb-116">Not supported.</span></span>|
|<span data-ttu-id="b2fbb-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="b2fbb-117">Application</span></span>|<span data-ttu-id="b2fbb-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b2fbb-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="b2fbb-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="b2fbb-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/windowsUpdateCatalogItems
```

## <a name="request-headers"></a><span data-ttu-id="b2fbb-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="b2fbb-120">Request headers</span></span>
|<span data-ttu-id="b2fbb-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="b2fbb-121">Header</span></span>|<span data-ttu-id="b2fbb-122">Значение</span><span class="sxs-lookup"><span data-stu-id="b2fbb-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b2fbb-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="b2fbb-123">Authorization</span></span>|<span data-ttu-id="b2fbb-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="b2fbb-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b2fbb-125">Accept</span><span class="sxs-lookup"><span data-stu-id="b2fbb-125">Accept</span></span>|<span data-ttu-id="b2fbb-126">application/json</span><span class="sxs-lookup"><span data-stu-id="b2fbb-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b2fbb-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="b2fbb-127">Request body</span></span>
<span data-ttu-id="b2fbb-128">В теле запроса укатите представление объекта windowsQualityUpdateCatalogItem в JSON.</span><span class="sxs-lookup"><span data-stu-id="b2fbb-128">In the request body, supply a JSON representation for the windowsQualityUpdateCatalogItem object.</span></span>

<span data-ttu-id="b2fbb-129">В следующей таблице показаны свойства, необходимые при создании объекта windowsQualityUpdateCatalogItem.</span><span class="sxs-lookup"><span data-stu-id="b2fbb-129">The following table shows the properties that are required when you create the windowsQualityUpdateCatalogItem.</span></span>

|<span data-ttu-id="b2fbb-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="b2fbb-130">Property</span></span>|<span data-ttu-id="b2fbb-131">Тип</span><span class="sxs-lookup"><span data-stu-id="b2fbb-131">Type</span></span>|<span data-ttu-id="b2fbb-132">Описание</span><span class="sxs-lookup"><span data-stu-id="b2fbb-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b2fbb-133">id</span><span class="sxs-lookup"><span data-stu-id="b2fbb-133">id</span></span>|<span data-ttu-id="b2fbb-134">String</span><span class="sxs-lookup"><span data-stu-id="b2fbb-134">String</span></span>|<span data-ttu-id="b2fbb-135">ИД элемента каталога. Наследуется [от windowsUpdateCatalogItem](../resources/intune-softwareupdate-windowsupdatecatalogitem.md)</span><span class="sxs-lookup"><span data-stu-id="b2fbb-135">The catalog item id. Inherited from [windowsUpdateCatalogItem](../resources/intune-softwareupdate-windowsupdatecatalogitem.md)</span></span>|
|<span data-ttu-id="b2fbb-136">displayName</span><span class="sxs-lookup"><span data-stu-id="b2fbb-136">displayName</span></span>|<span data-ttu-id="b2fbb-137">String</span><span class="sxs-lookup"><span data-stu-id="b2fbb-137">String</span></span>|<span data-ttu-id="b2fbb-138">Отображаемого имени элемента каталога.</span><span class="sxs-lookup"><span data-stu-id="b2fbb-138">The display name for the catalog item.</span></span> <span data-ttu-id="b2fbb-139">Наследуется [от windowsUpdateCatalogItem](../resources/intune-softwareupdate-windowsupdatecatalogitem.md)</span><span class="sxs-lookup"><span data-stu-id="b2fbb-139">Inherited from [windowsUpdateCatalogItem](../resources/intune-softwareupdate-windowsupdatecatalogitem.md)</span></span>|
|<span data-ttu-id="b2fbb-140">releaseDateTime</span><span class="sxs-lookup"><span data-stu-id="b2fbb-140">releaseDateTime</span></span>|<span data-ttu-id="b2fbb-141">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b2fbb-141">DateTimeOffset</span></span>|<span data-ttu-id="b2fbb-142">Дата выпуска элемента каталога. Наследуется от [windowsUpdateCatalogItem](../resources/intune-softwareupdate-windowsupdatecatalogitem.md)</span><span class="sxs-lookup"><span data-stu-id="b2fbb-142">The date the catalog item was released Inherited from [windowsUpdateCatalogItem](../resources/intune-softwareupdate-windowsupdatecatalogitem.md)</span></span>|
|<span data-ttu-id="b2fbb-143">kbArticleId</span><span class="sxs-lookup"><span data-stu-id="b2fbb-143">kbArticleId</span></span>|<span data-ttu-id="b2fbb-144">String</span><span class="sxs-lookup"><span data-stu-id="b2fbb-144">String</span></span>|<span data-ttu-id="b2fbb-145">ИД статьи базы знаний</span><span class="sxs-lookup"><span data-stu-id="b2fbb-145">Knowledge base article id</span></span>|
|<span data-ttu-id="b2fbb-146">classification</span><span class="sxs-lookup"><span data-stu-id="b2fbb-146">classification</span></span>|[<span data-ttu-id="b2fbb-147">windowsQualityUpdateClassification</span><span class="sxs-lookup"><span data-stu-id="b2fbb-147">windowsQualityUpdateClassification</span></span>](../resources/intune-softwareupdate-windowsqualityupdateclassification.md)|<span data-ttu-id="b2fbb-148">Классификация обновления качества.</span><span class="sxs-lookup"><span data-stu-id="b2fbb-148">Classification of the quality update.</span></span> <span data-ttu-id="b2fbb-149">Возможные значения: `all`, `security`, `nonSecurity`.</span><span class="sxs-lookup"><span data-stu-id="b2fbb-149">Possible values are: `all`, `security`, `nonSecurity`.</span></span>|
|<span data-ttu-id="b2fbb-150">isExpeditable</span><span class="sxs-lookup"><span data-stu-id="b2fbb-150">isExpeditable</span></span>|<span data-ttu-id="b2fbb-151">Boolean</span><span class="sxs-lookup"><span data-stu-id="b2fbb-151">Boolean</span></span>|<span data-ttu-id="b2fbb-152">Флаг, указывающий, является ли обновление квалификатором для ускорения</span><span class="sxs-lookup"><span data-stu-id="b2fbb-152">Flag indicating if update qualifies for expedite</span></span>|



## <a name="response"></a><span data-ttu-id="b2fbb-153">Отклик</span><span class="sxs-lookup"><span data-stu-id="b2fbb-153">Response</span></span>
<span data-ttu-id="b2fbb-154">В случае успеха этот метод возвращает код отклика и объект `201 Created` [windowsQualityUpdateCatalogItem](../resources/intune-softwareupdate-windowsqualityupdatecatalogitem.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="b2fbb-154">If successful, this method returns a `201 Created` response code and a [windowsQualityUpdateCatalogItem](../resources/intune-softwareupdate-windowsqualityupdatecatalogitem.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b2fbb-155">Пример</span><span class="sxs-lookup"><span data-stu-id="b2fbb-155">Example</span></span>

### <a name="request"></a><span data-ttu-id="b2fbb-156">Запрос</span><span class="sxs-lookup"><span data-stu-id="b2fbb-156">Request</span></span>
<span data-ttu-id="b2fbb-157">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="b2fbb-157">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/windowsUpdateCatalogItems
Content-type: application/json
Content-length: 272

{
  "@odata.type": "#microsoft.graph.windowsQualityUpdateCatalogItem",
  "displayName": "Display Name value",
  "releaseDateTime": "2017-01-01T00:01:34.7470482-08:00",
  "kbArticleId": "Kb Article Id value",
  "classification": "security",
  "isExpeditable": true
}
```

### <a name="response"></a><span data-ttu-id="b2fbb-158">Отклик</span><span class="sxs-lookup"><span data-stu-id="b2fbb-158">Response</span></span>
<span data-ttu-id="b2fbb-p104">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="b2fbb-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 321

{
  "@odata.type": "#microsoft.graph.windowsQualityUpdateCatalogItem",
  "id": "8eb831ba-31ba-8eb8-ba31-b88eba31b88e",
  "displayName": "Display Name value",
  "releaseDateTime": "2017-01-01T00:01:34.7470482-08:00",
  "kbArticleId": "Kb Article Id value",
  "classification": "security",
  "isExpeditable": true
}
```




