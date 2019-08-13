---
title: Обновление Манажедебуккатегори
description: Обновление свойств объекта Манажедебуккатегори.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: bb930180b22c734f0abb2b7be7450678ae48e350
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/13/2019
ms.locfileid: "36328328"
---
# <a name="update-managedebookcategory"></a><span data-ttu-id="c9842-103">Обновление Манажедебуккатегори</span><span class="sxs-lookup"><span data-stu-id="c9842-103">Update managedEBookCategory</span></span>

> <span data-ttu-id="c9842-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c9842-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c9842-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="c9842-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c9842-106">Обновление свойств объекта [манажедебуккатегори](../resources/intune-books-managedebookcategory.md) .</span><span class="sxs-lookup"><span data-stu-id="c9842-106">Update the properties of a [managedEBookCategory](../resources/intune-books-managedebookcategory.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="c9842-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="c9842-107">Prerequisites</span></span>
<span data-ttu-id="c9842-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c9842-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c9842-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c9842-110">Permission type</span></span>|<span data-ttu-id="c9842-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="c9842-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c9842-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c9842-112">Delegated (work or school account)</span></span>|<span data-ttu-id="c9842-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c9842-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="c9842-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c9842-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c9842-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c9842-115">Not supported.</span></span>|
|<span data-ttu-id="c9842-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="c9842-116">Application</span></span>|<span data-ttu-id="c9842-117">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c9842-117">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="c9842-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c9842-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/managedEBookCategories/{managedEBookCategoryId}
PATCH /deviceAppManagement/managedEBooks/{managedEBookId}/categories/{managedEBookCategoryId}
```

## <a name="request-headers"></a><span data-ttu-id="c9842-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="c9842-119">Request headers</span></span>
|<span data-ttu-id="c9842-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="c9842-120">Header</span></span>|<span data-ttu-id="c9842-121">Значение</span><span class="sxs-lookup"><span data-stu-id="c9842-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c9842-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="c9842-122">Authorization</span></span>|<span data-ttu-id="c9842-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c9842-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c9842-124">Accept</span><span class="sxs-lookup"><span data-stu-id="c9842-124">Accept</span></span>|<span data-ttu-id="c9842-125">application/json</span><span class="sxs-lookup"><span data-stu-id="c9842-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c9842-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="c9842-126">Request body</span></span>
<span data-ttu-id="c9842-127">В тексте запроса добавьте представление объекта [манажедебуккатегори](../resources/intune-books-managedebookcategory.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="c9842-127">In the request body, supply a JSON representation for the [managedEBookCategory](../resources/intune-books-managedebookcategory.md) object.</span></span>

<span data-ttu-id="c9842-128">В следующей таблице приведены свойства, необходимые при создании [манажедебуккатегори](../resources/intune-books-managedebookcategory.md).</span><span class="sxs-lookup"><span data-stu-id="c9842-128">The following table shows the properties that are required when you create the [managedEBookCategory](../resources/intune-books-managedebookcategory.md).</span></span>

|<span data-ttu-id="c9842-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="c9842-129">Property</span></span>|<span data-ttu-id="c9842-130">Тип</span><span class="sxs-lookup"><span data-stu-id="c9842-130">Type</span></span>|<span data-ttu-id="c9842-131">Описание</span><span class="sxs-lookup"><span data-stu-id="c9842-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c9842-132">id</span><span class="sxs-lookup"><span data-stu-id="c9842-132">id</span></span>|<span data-ttu-id="c9842-133">String</span><span class="sxs-lookup"><span data-stu-id="c9842-133">String</span></span>|<span data-ttu-id="c9842-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="c9842-134">The key of the entity.</span></span>|
|<span data-ttu-id="c9842-135">displayName</span><span class="sxs-lookup"><span data-stu-id="c9842-135">displayName</span></span>|<span data-ttu-id="c9842-136">Строка</span><span class="sxs-lookup"><span data-stu-id="c9842-136">String</span></span>|<span data-ttu-id="c9842-137">Имя категории электронной книги.</span><span class="sxs-lookup"><span data-stu-id="c9842-137">The name of the eBook category.</span></span>|
|<span data-ttu-id="c9842-138">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="c9842-138">lastModifiedDateTime</span></span>|<span data-ttu-id="c9842-139">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c9842-139">DateTimeOffset</span></span>|<span data-ttu-id="c9842-140">Дата и время последнего изменения Манажедебуккатегори.</span><span class="sxs-lookup"><span data-stu-id="c9842-140">The date and time the ManagedEBookCategory was last modified.</span></span>|



## <a name="response"></a><span data-ttu-id="c9842-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="c9842-141">Response</span></span>
<span data-ttu-id="c9842-142">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [манажедебуккатегори](../resources/intune-books-managedebookcategory.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="c9842-142">If successful, this method returns a `200 OK` response code and an updated [managedEBookCategory](../resources/intune-books-managedebookcategory.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c9842-143">Пример</span><span class="sxs-lookup"><span data-stu-id="c9842-143">Example</span></span>

### <a name="request"></a><span data-ttu-id="c9842-144">Запрос</span><span class="sxs-lookup"><span data-stu-id="c9842-144">Request</span></span>
<span data-ttu-id="c9842-145">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="c9842-145">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/managedEBookCategories/{managedEBookCategoryId}
Content-type: application/json
Content-length: 102

{
  "@odata.type": "#microsoft.graph.managedEBookCategory",
  "displayName": "Display Name value"
}
```

### <a name="response"></a><span data-ttu-id="c9842-146">Отклик</span><span class="sxs-lookup"><span data-stu-id="c9842-146">Response</span></span>
<span data-ttu-id="c9842-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="c9842-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 215

{
  "@odata.type": "#microsoft.graph.managedEBookCategory",
  "id": "3c71fb14-fb14-3c71-14fb-713c14fb713c",
  "displayName": "Display Name value",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00"
}
```






