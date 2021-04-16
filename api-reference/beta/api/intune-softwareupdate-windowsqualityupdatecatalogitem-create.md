---
title: Создание windowsQualityUpdateCatalogItem
description: Создайте новый объект WindowsQualityUpdateCatalogItem.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: aec5d998ed02c946059816d164188bb566ddec7e
ms.sourcegitcommit: ed45b5ce0583dfa4d12f7cb0b3ac0c5aeb2318d4
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/16/2021
ms.locfileid: "51866883"
---
# <a name="create-windowsqualityupdatecatalogitem"></a><span data-ttu-id="f2b20-103">Создание windowsQualityUpdateCatalogItem</span><span class="sxs-lookup"><span data-stu-id="f2b20-103">Create windowsQualityUpdateCatalogItem</span></span>

<span data-ttu-id="f2b20-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f2b20-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="f2b20-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f2b20-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f2b20-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="f2b20-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f2b20-107">Создайте [новый объект WindowsQualityUpdateCatalogItem.](../resources/intune-softwareupdate-windowsqualityupdatecatalogitem.md)</span><span class="sxs-lookup"><span data-stu-id="f2b20-107">Create a new [windowsQualityUpdateCatalogItem](../resources/intune-softwareupdate-windowsqualityupdatecatalogitem.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f2b20-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="f2b20-108">Prerequisites</span></span>
<span data-ttu-id="f2b20-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f2b20-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f2b20-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f2b20-111">Permission type</span></span>|<span data-ttu-id="f2b20-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="f2b20-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f2b20-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f2b20-113">Delegated (work or school account)</span></span>|<span data-ttu-id="f2b20-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f2b20-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="f2b20-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f2b20-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f2b20-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f2b20-116">Not supported.</span></span>|
|<span data-ttu-id="f2b20-117">Для приложения</span><span class="sxs-lookup"><span data-stu-id="f2b20-117">Application</span></span>|<span data-ttu-id="f2b20-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f2b20-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="f2b20-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f2b20-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/windowsUpdateCatalogItems
```

## <a name="request-headers"></a><span data-ttu-id="f2b20-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="f2b20-120">Request headers</span></span>
|<span data-ttu-id="f2b20-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="f2b20-121">Header</span></span>|<span data-ttu-id="f2b20-122">Значение</span><span class="sxs-lookup"><span data-stu-id="f2b20-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f2b20-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="f2b20-123">Authorization</span></span>|<span data-ttu-id="f2b20-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="f2b20-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f2b20-125">Accept</span><span class="sxs-lookup"><span data-stu-id="f2b20-125">Accept</span></span>|<span data-ttu-id="f2b20-126">application/json</span><span class="sxs-lookup"><span data-stu-id="f2b20-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f2b20-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="f2b20-127">Request body</span></span>
<span data-ttu-id="f2b20-128">В теле запроса поставляем представление JSON для объекта WindowsQualityUpdateCatalogItem.</span><span class="sxs-lookup"><span data-stu-id="f2b20-128">In the request body, supply a JSON representation for the windowsQualityUpdateCatalogItem object.</span></span>

<span data-ttu-id="f2b20-129">В следующей таблице показаны свойства, необходимые при создании windowsQualityUpdateCatalogItem.</span><span class="sxs-lookup"><span data-stu-id="f2b20-129">The following table shows the properties that are required when you create the windowsQualityUpdateCatalogItem.</span></span>

|<span data-ttu-id="f2b20-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="f2b20-130">Property</span></span>|<span data-ttu-id="f2b20-131">Тип</span><span class="sxs-lookup"><span data-stu-id="f2b20-131">Type</span></span>|<span data-ttu-id="f2b20-132">Описание</span><span class="sxs-lookup"><span data-stu-id="f2b20-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f2b20-133">id</span><span class="sxs-lookup"><span data-stu-id="f2b20-133">id</span></span>|<span data-ttu-id="f2b20-134">String</span><span class="sxs-lookup"><span data-stu-id="f2b20-134">String</span></span>|<span data-ttu-id="f2b20-135">ID элемента каталога. Унаследованный от [windowsUpdateCatalogItem](../resources/intune-softwareupdate-windowsupdatecatalogitem.md)</span><span class="sxs-lookup"><span data-stu-id="f2b20-135">The catalog item id. Inherited from [windowsUpdateCatalogItem](../resources/intune-softwareupdate-windowsupdatecatalogitem.md)</span></span>|
|<span data-ttu-id="f2b20-136">displayName</span><span class="sxs-lookup"><span data-stu-id="f2b20-136">displayName</span></span>|<span data-ttu-id="f2b20-137">String</span><span class="sxs-lookup"><span data-stu-id="f2b20-137">String</span></span>|<span data-ttu-id="f2b20-138">Имя отображения элемента каталога.</span><span class="sxs-lookup"><span data-stu-id="f2b20-138">The display name for the catalog item.</span></span> <span data-ttu-id="f2b20-139">Унаследованный от [windowsUpdateCatalogItem](../resources/intune-softwareupdate-windowsupdatecatalogitem.md)</span><span class="sxs-lookup"><span data-stu-id="f2b20-139">Inherited from [windowsUpdateCatalogItem](../resources/intune-softwareupdate-windowsupdatecatalogitem.md)</span></span>|
|<span data-ttu-id="f2b20-140">releaseDateTime</span><span class="sxs-lookup"><span data-stu-id="f2b20-140">releaseDateTime</span></span>|<span data-ttu-id="f2b20-141">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f2b20-141">DateTimeOffset</span></span>|<span data-ttu-id="f2b20-142">Дата выпуска элемента каталога, наследуемого [из windowsUpdateCatalogItem](../resources/intune-softwareupdate-windowsupdatecatalogitem.md)</span><span class="sxs-lookup"><span data-stu-id="f2b20-142">The date the catalog item was released Inherited from [windowsUpdateCatalogItem](../resources/intune-softwareupdate-windowsupdatecatalogitem.md)</span></span>|
|<span data-ttu-id="f2b20-143">endOfSupportDate</span><span class="sxs-lookup"><span data-stu-id="f2b20-143">endOfSupportDate</span></span>|<span data-ttu-id="f2b20-144">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f2b20-144">DateTimeOffset</span></span>|<span data-ttu-id="f2b20-145">Последняя поддерживаемая дата для элемента каталога, наследуемого [из windowsUpdateCatalogItem](../resources/intune-softwareupdate-windowsupdatecatalogitem.md)</span><span class="sxs-lookup"><span data-stu-id="f2b20-145">The last supported date for a catalog item Inherited from [windowsUpdateCatalogItem](../resources/intune-softwareupdate-windowsupdatecatalogitem.md)</span></span>|
|<span data-ttu-id="f2b20-146">kbArticleId</span><span class="sxs-lookup"><span data-stu-id="f2b20-146">kbArticleId</span></span>|<span data-ttu-id="f2b20-147">String</span><span class="sxs-lookup"><span data-stu-id="f2b20-147">String</span></span>|<span data-ttu-id="f2b20-148">ID статьи базы знаний</span><span class="sxs-lookup"><span data-stu-id="f2b20-148">Knowledge base article id</span></span>|
|<span data-ttu-id="f2b20-149">classification</span><span class="sxs-lookup"><span data-stu-id="f2b20-149">classification</span></span>|[<span data-ttu-id="f2b20-150">windowsQualityUpdateClassification</span><span class="sxs-lookup"><span data-stu-id="f2b20-150">windowsQualityUpdateClassification</span></span>](../resources/intune-softwareupdate-windowsqualityupdateclassification.md)|<span data-ttu-id="f2b20-151">Классификация обновления качества.</span><span class="sxs-lookup"><span data-stu-id="f2b20-151">Classification of the quality update.</span></span> <span data-ttu-id="f2b20-152">Возможные значения: `all`, `security`, `nonSecurity`.</span><span class="sxs-lookup"><span data-stu-id="f2b20-152">Possible values are: `all`, `security`, `nonSecurity`.</span></span>|
|<span data-ttu-id="f2b20-153">isExpeditable</span><span class="sxs-lookup"><span data-stu-id="f2b20-153">isExpeditable</span></span>|<span data-ttu-id="f2b20-154">Логический</span><span class="sxs-lookup"><span data-stu-id="f2b20-154">Boolean</span></span>|<span data-ttu-id="f2b20-155">Флаг, указывающий, имеет ли обновление право на ускорение</span><span class="sxs-lookup"><span data-stu-id="f2b20-155">Flag indicating if update qualifies for expedite</span></span>|



## <a name="response"></a><span data-ttu-id="f2b20-156">Отклик</span><span class="sxs-lookup"><span data-stu-id="f2b20-156">Response</span></span>
<span data-ttu-id="f2b20-157">В случае успеха этот метод возвращает код отклика и `201 Created` [объект WindowsQualityUpdateCatalogItem](../resources/intune-softwareupdate-windowsqualityupdatecatalogitem.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="f2b20-157">If successful, this method returns a `201 Created` response code and a [windowsQualityUpdateCatalogItem](../resources/intune-softwareupdate-windowsqualityupdatecatalogitem.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f2b20-158">Пример</span><span class="sxs-lookup"><span data-stu-id="f2b20-158">Example</span></span>

### <a name="request"></a><span data-ttu-id="f2b20-159">Запрос</span><span class="sxs-lookup"><span data-stu-id="f2b20-159">Request</span></span>
<span data-ttu-id="f2b20-160">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="f2b20-160">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/windowsUpdateCatalogItems
Content-type: application/json
Content-length: 332

{
  "@odata.type": "#microsoft.graph.windowsQualityUpdateCatalogItem",
  "displayName": "Display Name value",
  "releaseDateTime": "2017-01-01T00:01:34.7470482-08:00",
  "endOfSupportDate": "2017-01-01T00:02:08.3437725-08:00",
  "kbArticleId": "Kb Article Id value",
  "classification": "security",
  "isExpeditable": true
}
```

### <a name="response"></a><span data-ttu-id="f2b20-161">Отклик</span><span class="sxs-lookup"><span data-stu-id="f2b20-161">Response</span></span>
<span data-ttu-id="f2b20-p104">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="f2b20-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 381

{
  "@odata.type": "#microsoft.graph.windowsQualityUpdateCatalogItem",
  "id": "8eb831ba-31ba-8eb8-ba31-b88eba31b88e",
  "displayName": "Display Name value",
  "releaseDateTime": "2017-01-01T00:01:34.7470482-08:00",
  "endOfSupportDate": "2017-01-01T00:02:08.3437725-08:00",
  "kbArticleId": "Kb Article Id value",
  "classification": "security",
  "isExpeditable": true
}
```




