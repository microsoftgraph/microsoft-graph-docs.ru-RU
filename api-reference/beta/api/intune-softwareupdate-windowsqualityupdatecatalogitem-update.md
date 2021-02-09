---
title: Обновление windowsQualityUpdateCatalogItem
description: Обновление свойств объекта windowsQualityUpdateCatalogItem.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 732df024970a1e096e99e902a9b9a737a92ea3fb
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/09/2021
ms.locfileid: "50160760"
---
# <a name="update-windowsqualityupdatecatalogitem"></a><span data-ttu-id="846b4-103">Обновление windowsQualityUpdateCatalogItem</span><span class="sxs-lookup"><span data-stu-id="846b4-103">Update windowsQualityUpdateCatalogItem</span></span>

<span data-ttu-id="846b4-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="846b4-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="846b4-105">**Важно!** API Microsoft Graph в бета-версии могут изменяться; использование в производственной области не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="846b4-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="846b4-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="846b4-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="846b4-107">Обновление свойств объекта [windowsQualityUpdateCatalogItem.](../resources/intune-softwareupdate-windowsqualityupdatecatalogitem.md)</span><span class="sxs-lookup"><span data-stu-id="846b4-107">Update the properties of a [windowsQualityUpdateCatalogItem](../resources/intune-softwareupdate-windowsqualityupdatecatalogitem.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="846b4-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="846b4-108">Prerequisites</span></span>
<span data-ttu-id="846b4-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="846b4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="846b4-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="846b4-111">Permission type</span></span>|<span data-ttu-id="846b4-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="846b4-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="846b4-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="846b4-113">Delegated (work or school account)</span></span>|<span data-ttu-id="846b4-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="846b4-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="846b4-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="846b4-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="846b4-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="846b4-116">Not supported.</span></span>|
|<span data-ttu-id="846b4-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="846b4-117">Application</span></span>|<span data-ttu-id="846b4-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="846b4-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="846b4-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="846b4-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/windowsUpdateCatalogItems/{windowsUpdateCatalogItemId}
```

## <a name="request-headers"></a><span data-ttu-id="846b4-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="846b4-120">Request headers</span></span>
|<span data-ttu-id="846b4-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="846b4-121">Header</span></span>|<span data-ttu-id="846b4-122">Значение</span><span class="sxs-lookup"><span data-stu-id="846b4-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="846b4-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="846b4-123">Authorization</span></span>|<span data-ttu-id="846b4-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="846b4-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="846b4-125">Accept</span><span class="sxs-lookup"><span data-stu-id="846b4-125">Accept</span></span>|<span data-ttu-id="846b4-126">application/json</span><span class="sxs-lookup"><span data-stu-id="846b4-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="846b4-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="846b4-127">Request body</span></span>
<span data-ttu-id="846b4-128">В теле запроса укатите представление объекта [windowsQualityUpdateCatalogItem](../resources/intune-softwareupdate-windowsqualityupdatecatalogitem.md) в JSON.</span><span class="sxs-lookup"><span data-stu-id="846b4-128">In the request body, supply a JSON representation for the [windowsQualityUpdateCatalogItem](../resources/intune-softwareupdate-windowsqualityupdatecatalogitem.md) object.</span></span>

<span data-ttu-id="846b4-129">В следующей таблице показаны свойства, необходимые при создании [объекта windowsQualityUpdateCatalogItem.](../resources/intune-softwareupdate-windowsqualityupdatecatalogitem.md)</span><span class="sxs-lookup"><span data-stu-id="846b4-129">The following table shows the properties that are required when you create the [windowsQualityUpdateCatalogItem](../resources/intune-softwareupdate-windowsqualityupdatecatalogitem.md).</span></span>

|<span data-ttu-id="846b4-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="846b4-130">Property</span></span>|<span data-ttu-id="846b4-131">Тип</span><span class="sxs-lookup"><span data-stu-id="846b4-131">Type</span></span>|<span data-ttu-id="846b4-132">Описание</span><span class="sxs-lookup"><span data-stu-id="846b4-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="846b4-133">id</span><span class="sxs-lookup"><span data-stu-id="846b4-133">id</span></span>|<span data-ttu-id="846b4-134">String</span><span class="sxs-lookup"><span data-stu-id="846b4-134">String</span></span>|<span data-ttu-id="846b4-135">ИД элемента каталога. Наследуется [от windowsUpdateCatalogItem](../resources/intune-softwareupdate-windowsupdatecatalogitem.md)</span><span class="sxs-lookup"><span data-stu-id="846b4-135">The catalog item id. Inherited from [windowsUpdateCatalogItem](../resources/intune-softwareupdate-windowsupdatecatalogitem.md)</span></span>|
|<span data-ttu-id="846b4-136">displayName</span><span class="sxs-lookup"><span data-stu-id="846b4-136">displayName</span></span>|<span data-ttu-id="846b4-137">String</span><span class="sxs-lookup"><span data-stu-id="846b4-137">String</span></span>|<span data-ttu-id="846b4-138">Отображаемого имени элемента каталога.</span><span class="sxs-lookup"><span data-stu-id="846b4-138">The display name for the catalog item.</span></span> <span data-ttu-id="846b4-139">Наследуется [от windowsUpdateCatalogItem](../resources/intune-softwareupdate-windowsupdatecatalogitem.md)</span><span class="sxs-lookup"><span data-stu-id="846b4-139">Inherited from [windowsUpdateCatalogItem](../resources/intune-softwareupdate-windowsupdatecatalogitem.md)</span></span>|
|<span data-ttu-id="846b4-140">releaseDateTime</span><span class="sxs-lookup"><span data-stu-id="846b4-140">releaseDateTime</span></span>|<span data-ttu-id="846b4-141">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="846b4-141">DateTimeOffset</span></span>|<span data-ttu-id="846b4-142">Дата выпуска элемента каталога. Наследуется от [windowsUpdateCatalogItem](../resources/intune-softwareupdate-windowsupdatecatalogitem.md)</span><span class="sxs-lookup"><span data-stu-id="846b4-142">The date the catalog item was released Inherited from [windowsUpdateCatalogItem](../resources/intune-softwareupdate-windowsupdatecatalogitem.md)</span></span>|
|<span data-ttu-id="846b4-143">kbArticleId</span><span class="sxs-lookup"><span data-stu-id="846b4-143">kbArticleId</span></span>|<span data-ttu-id="846b4-144">String</span><span class="sxs-lookup"><span data-stu-id="846b4-144">String</span></span>|<span data-ttu-id="846b4-145">ИД статьи базы знаний</span><span class="sxs-lookup"><span data-stu-id="846b4-145">Knowledge base article id</span></span>|
|<span data-ttu-id="846b4-146">classification</span><span class="sxs-lookup"><span data-stu-id="846b4-146">classification</span></span>|[<span data-ttu-id="846b4-147">windowsQualityUpdateClassification</span><span class="sxs-lookup"><span data-stu-id="846b4-147">windowsQualityUpdateClassification</span></span>](../resources/intune-softwareupdate-windowsqualityupdateclassification.md)|<span data-ttu-id="846b4-148">Классификация обновления качества.</span><span class="sxs-lookup"><span data-stu-id="846b4-148">Classification of the quality update.</span></span> <span data-ttu-id="846b4-149">Возможные значения: `all`, `security`, `nonSecurity`.</span><span class="sxs-lookup"><span data-stu-id="846b4-149">Possible values are: `all`, `security`, `nonSecurity`.</span></span>|
|<span data-ttu-id="846b4-150">isExpeditable</span><span class="sxs-lookup"><span data-stu-id="846b4-150">isExpeditable</span></span>|<span data-ttu-id="846b4-151">Boolean</span><span class="sxs-lookup"><span data-stu-id="846b4-151">Boolean</span></span>|<span data-ttu-id="846b4-152">Флаг, указывающий, является ли обновление квалификатором для ускорения</span><span class="sxs-lookup"><span data-stu-id="846b4-152">Flag indicating if update qualifies for expedite</span></span>|



## <a name="response"></a><span data-ttu-id="846b4-153">Отклик</span><span class="sxs-lookup"><span data-stu-id="846b4-153">Response</span></span>
<span data-ttu-id="846b4-154">В случае успеха этот метод возвращает код отклика и обновленный объект `200 OK` [windowsQualityUpdateCatalogItem](../resources/intune-softwareupdate-windowsqualityupdatecatalogitem.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="846b4-154">If successful, this method returns a `200 OK` response code and an updated [windowsQualityUpdateCatalogItem](../resources/intune-softwareupdate-windowsqualityupdatecatalogitem.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="846b4-155">Пример</span><span class="sxs-lookup"><span data-stu-id="846b4-155">Example</span></span>

### <a name="request"></a><span data-ttu-id="846b4-156">Запрос</span><span class="sxs-lookup"><span data-stu-id="846b4-156">Request</span></span>
<span data-ttu-id="846b4-157">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="846b4-157">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/windowsUpdateCatalogItems/{windowsUpdateCatalogItemId}
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

### <a name="response"></a><span data-ttu-id="846b4-158">Отклик</span><span class="sxs-lookup"><span data-stu-id="846b4-158">Response</span></span>
<span data-ttu-id="846b4-p104">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="846b4-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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




