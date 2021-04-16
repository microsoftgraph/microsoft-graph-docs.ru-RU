---
title: Обновление windowsQualityUpdateCatalogItem
description: Обновление свойств объекта windowsQualityUpdateCatalogItem.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 5dcaadfea931ef5d6e9a1fce5bc9e948269d390b
ms.sourcegitcommit: ed45b5ce0583dfa4d12f7cb0b3ac0c5aeb2318d4
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/16/2021
ms.locfileid: "51868043"
---
# <a name="update-windowsqualityupdatecatalogitem"></a><span data-ttu-id="b4dde-103">Обновление windowsQualityUpdateCatalogItem</span><span class="sxs-lookup"><span data-stu-id="b4dde-103">Update windowsQualityUpdateCatalogItem</span></span>

<span data-ttu-id="b4dde-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b4dde-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="b4dde-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b4dde-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b4dde-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="b4dde-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b4dde-107">Обновление свойств объекта [windowsQualityUpdateCatalogItem.](../resources/intune-softwareupdate-windowsqualityupdatecatalogitem.md)</span><span class="sxs-lookup"><span data-stu-id="b4dde-107">Update the properties of a [windowsQualityUpdateCatalogItem](../resources/intune-softwareupdate-windowsqualityupdatecatalogitem.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="b4dde-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="b4dde-108">Prerequisites</span></span>
<span data-ttu-id="b4dde-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b4dde-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b4dde-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="b4dde-111">Permission type</span></span>|<span data-ttu-id="b4dde-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="b4dde-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b4dde-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="b4dde-113">Delegated (work or school account)</span></span>|<span data-ttu-id="b4dde-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b4dde-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="b4dde-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="b4dde-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b4dde-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b4dde-116">Not supported.</span></span>|
|<span data-ttu-id="b4dde-117">Для приложения</span><span class="sxs-lookup"><span data-stu-id="b4dde-117">Application</span></span>|<span data-ttu-id="b4dde-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b4dde-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="b4dde-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="b4dde-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/windowsUpdateCatalogItems/{windowsUpdateCatalogItemId}
```

## <a name="request-headers"></a><span data-ttu-id="b4dde-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="b4dde-120">Request headers</span></span>
|<span data-ttu-id="b4dde-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="b4dde-121">Header</span></span>|<span data-ttu-id="b4dde-122">Значение</span><span class="sxs-lookup"><span data-stu-id="b4dde-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b4dde-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="b4dde-123">Authorization</span></span>|<span data-ttu-id="b4dde-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="b4dde-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b4dde-125">Accept</span><span class="sxs-lookup"><span data-stu-id="b4dde-125">Accept</span></span>|<span data-ttu-id="b4dde-126">application/json</span><span class="sxs-lookup"><span data-stu-id="b4dde-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b4dde-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="b4dde-127">Request body</span></span>
<span data-ttu-id="b4dde-128">В теле запроса поставляем представление JSON для [объекта WindowsQualityUpdateCatalogItem.](../resources/intune-softwareupdate-windowsqualityupdatecatalogitem.md)</span><span class="sxs-lookup"><span data-stu-id="b4dde-128">In the request body, supply a JSON representation for the [windowsQualityUpdateCatalogItem](../resources/intune-softwareupdate-windowsqualityupdatecatalogitem.md) object.</span></span>

<span data-ttu-id="b4dde-129">В следующей таблице показаны свойства, необходимые при создании [windowsQualityUpdateCatalogItem.](../resources/intune-softwareupdate-windowsqualityupdatecatalogitem.md)</span><span class="sxs-lookup"><span data-stu-id="b4dde-129">The following table shows the properties that are required when you create the [windowsQualityUpdateCatalogItem](../resources/intune-softwareupdate-windowsqualityupdatecatalogitem.md).</span></span>

|<span data-ttu-id="b4dde-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="b4dde-130">Property</span></span>|<span data-ttu-id="b4dde-131">Тип</span><span class="sxs-lookup"><span data-stu-id="b4dde-131">Type</span></span>|<span data-ttu-id="b4dde-132">Описание</span><span class="sxs-lookup"><span data-stu-id="b4dde-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b4dde-133">id</span><span class="sxs-lookup"><span data-stu-id="b4dde-133">id</span></span>|<span data-ttu-id="b4dde-134">String</span><span class="sxs-lookup"><span data-stu-id="b4dde-134">String</span></span>|<span data-ttu-id="b4dde-135">ID элемента каталога. Унаследованный от [windowsUpdateCatalogItem](../resources/intune-softwareupdate-windowsupdatecatalogitem.md)</span><span class="sxs-lookup"><span data-stu-id="b4dde-135">The catalog item id. Inherited from [windowsUpdateCatalogItem](../resources/intune-softwareupdate-windowsupdatecatalogitem.md)</span></span>|
|<span data-ttu-id="b4dde-136">displayName</span><span class="sxs-lookup"><span data-stu-id="b4dde-136">displayName</span></span>|<span data-ttu-id="b4dde-137">String</span><span class="sxs-lookup"><span data-stu-id="b4dde-137">String</span></span>|<span data-ttu-id="b4dde-138">Имя отображения элемента каталога.</span><span class="sxs-lookup"><span data-stu-id="b4dde-138">The display name for the catalog item.</span></span> <span data-ttu-id="b4dde-139">Унаследованный от [windowsUpdateCatalogItem](../resources/intune-softwareupdate-windowsupdatecatalogitem.md)</span><span class="sxs-lookup"><span data-stu-id="b4dde-139">Inherited from [windowsUpdateCatalogItem](../resources/intune-softwareupdate-windowsupdatecatalogitem.md)</span></span>|
|<span data-ttu-id="b4dde-140">releaseDateTime</span><span class="sxs-lookup"><span data-stu-id="b4dde-140">releaseDateTime</span></span>|<span data-ttu-id="b4dde-141">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b4dde-141">DateTimeOffset</span></span>|<span data-ttu-id="b4dde-142">Дата выпуска элемента каталога, наследуемого [из windowsUpdateCatalogItem](../resources/intune-softwareupdate-windowsupdatecatalogitem.md)</span><span class="sxs-lookup"><span data-stu-id="b4dde-142">The date the catalog item was released Inherited from [windowsUpdateCatalogItem](../resources/intune-softwareupdate-windowsupdatecatalogitem.md)</span></span>|
|<span data-ttu-id="b4dde-143">endOfSupportDate</span><span class="sxs-lookup"><span data-stu-id="b4dde-143">endOfSupportDate</span></span>|<span data-ttu-id="b4dde-144">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b4dde-144">DateTimeOffset</span></span>|<span data-ttu-id="b4dde-145">Последняя поддерживаемая дата для элемента каталога, наследуемого [из windowsUpdateCatalogItem](../resources/intune-softwareupdate-windowsupdatecatalogitem.md)</span><span class="sxs-lookup"><span data-stu-id="b4dde-145">The last supported date for a catalog item Inherited from [windowsUpdateCatalogItem](../resources/intune-softwareupdate-windowsupdatecatalogitem.md)</span></span>|
|<span data-ttu-id="b4dde-146">kbArticleId</span><span class="sxs-lookup"><span data-stu-id="b4dde-146">kbArticleId</span></span>|<span data-ttu-id="b4dde-147">String</span><span class="sxs-lookup"><span data-stu-id="b4dde-147">String</span></span>|<span data-ttu-id="b4dde-148">ID статьи базы знаний</span><span class="sxs-lookup"><span data-stu-id="b4dde-148">Knowledge base article id</span></span>|
|<span data-ttu-id="b4dde-149">classification</span><span class="sxs-lookup"><span data-stu-id="b4dde-149">classification</span></span>|[<span data-ttu-id="b4dde-150">windowsQualityUpdateClassification</span><span class="sxs-lookup"><span data-stu-id="b4dde-150">windowsQualityUpdateClassification</span></span>](../resources/intune-softwareupdate-windowsqualityupdateclassification.md)|<span data-ttu-id="b4dde-151">Классификация обновления качества.</span><span class="sxs-lookup"><span data-stu-id="b4dde-151">Classification of the quality update.</span></span> <span data-ttu-id="b4dde-152">Возможные значения: `all`, `security`, `nonSecurity`.</span><span class="sxs-lookup"><span data-stu-id="b4dde-152">Possible values are: `all`, `security`, `nonSecurity`.</span></span>|
|<span data-ttu-id="b4dde-153">isExpeditable</span><span class="sxs-lookup"><span data-stu-id="b4dde-153">isExpeditable</span></span>|<span data-ttu-id="b4dde-154">Логический</span><span class="sxs-lookup"><span data-stu-id="b4dde-154">Boolean</span></span>|<span data-ttu-id="b4dde-155">Флаг, указывающий, имеет ли обновление право на ускорение</span><span class="sxs-lookup"><span data-stu-id="b4dde-155">Flag indicating if update qualifies for expedite</span></span>|



## <a name="response"></a><span data-ttu-id="b4dde-156">Отклик</span><span class="sxs-lookup"><span data-stu-id="b4dde-156">Response</span></span>
<span data-ttu-id="b4dde-157">В случае успешной работы этот метод возвращает код отклика и обновленный `200 OK` [объект WindowsQualityUpdateCatalogItem](../resources/intune-softwareupdate-windowsqualityupdatecatalogitem.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="b4dde-157">If successful, this method returns a `200 OK` response code and an updated [windowsQualityUpdateCatalogItem](../resources/intune-softwareupdate-windowsqualityupdatecatalogitem.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b4dde-158">Пример</span><span class="sxs-lookup"><span data-stu-id="b4dde-158">Example</span></span>

### <a name="request"></a><span data-ttu-id="b4dde-159">Запрос</span><span class="sxs-lookup"><span data-stu-id="b4dde-159">Request</span></span>
<span data-ttu-id="b4dde-160">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="b4dde-160">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/windowsUpdateCatalogItems/{windowsUpdateCatalogItemId}
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

### <a name="response"></a><span data-ttu-id="b4dde-161">Отклик</span><span class="sxs-lookup"><span data-stu-id="b4dde-161">Response</span></span>
<span data-ttu-id="b4dde-p104">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="b4dde-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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




