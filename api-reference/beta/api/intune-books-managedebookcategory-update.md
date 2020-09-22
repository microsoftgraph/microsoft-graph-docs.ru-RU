---
title: Обновление Манажедебуккатегори
description: Обновление свойств объекта Манажедебуккатегори.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: fc75de0475ed7f7070ba7312959b29ca5460a840
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "47975439"
---
# <a name="update-managedebookcategory"></a><span data-ttu-id="a86d0-103">Обновление Манажедебуккатегори</span><span class="sxs-lookup"><span data-stu-id="a86d0-103">Update managedEBookCategory</span></span>

<span data-ttu-id="a86d0-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a86d0-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="a86d0-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a86d0-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a86d0-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="a86d0-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a86d0-107">Обновление свойств объекта [манажедебуккатегори](../resources/intune-books-managedebookcategory.md) .</span><span class="sxs-lookup"><span data-stu-id="a86d0-107">Update the properties of a [managedEBookCategory](../resources/intune-books-managedebookcategory.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a86d0-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="a86d0-108">Prerequisites</span></span>
<span data-ttu-id="a86d0-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a86d0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a86d0-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="a86d0-111">Permission type</span></span>|<span data-ttu-id="a86d0-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="a86d0-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a86d0-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a86d0-113">Delegated (work or school account)</span></span>|<span data-ttu-id="a86d0-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a86d0-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="a86d0-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a86d0-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a86d0-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a86d0-116">Not supported.</span></span>|
|<span data-ttu-id="a86d0-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="a86d0-117">Application</span></span>|<span data-ttu-id="a86d0-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a86d0-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="a86d0-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a86d0-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/managedEBookCategories/{managedEBookCategoryId}
PATCH /deviceAppManagement/managedEBooks/{managedEBookId}/categories/{managedEBookCategoryId}
```

## <a name="request-headers"></a><span data-ttu-id="a86d0-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="a86d0-120">Request headers</span></span>
|<span data-ttu-id="a86d0-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="a86d0-121">Header</span></span>|<span data-ttu-id="a86d0-122">Значение</span><span class="sxs-lookup"><span data-stu-id="a86d0-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a86d0-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="a86d0-123">Authorization</span></span>|<span data-ttu-id="a86d0-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="a86d0-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a86d0-125">Accept</span><span class="sxs-lookup"><span data-stu-id="a86d0-125">Accept</span></span>|<span data-ttu-id="a86d0-126">application/json</span><span class="sxs-lookup"><span data-stu-id="a86d0-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a86d0-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="a86d0-127">Request body</span></span>
<span data-ttu-id="a86d0-128">В тексте запроса добавьте представление объекта [манажедебуккатегори](../resources/intune-books-managedebookcategory.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="a86d0-128">In the request body, supply a JSON representation for the [managedEBookCategory](../resources/intune-books-managedebookcategory.md) object.</span></span>

<span data-ttu-id="a86d0-129">В следующей таблице приведены свойства, необходимые при создании [манажедебуккатегори](../resources/intune-books-managedebookcategory.md).</span><span class="sxs-lookup"><span data-stu-id="a86d0-129">The following table shows the properties that are required when you create the [managedEBookCategory](../resources/intune-books-managedebookcategory.md).</span></span>

|<span data-ttu-id="a86d0-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="a86d0-130">Property</span></span>|<span data-ttu-id="a86d0-131">Тип</span><span class="sxs-lookup"><span data-stu-id="a86d0-131">Type</span></span>|<span data-ttu-id="a86d0-132">Описание</span><span class="sxs-lookup"><span data-stu-id="a86d0-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a86d0-133">id</span><span class="sxs-lookup"><span data-stu-id="a86d0-133">id</span></span>|<span data-ttu-id="a86d0-134">String</span><span class="sxs-lookup"><span data-stu-id="a86d0-134">String</span></span>|<span data-ttu-id="a86d0-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="a86d0-135">The key of the entity.</span></span>|
|<span data-ttu-id="a86d0-136">displayName</span><span class="sxs-lookup"><span data-stu-id="a86d0-136">displayName</span></span>|<span data-ttu-id="a86d0-137">String</span><span class="sxs-lookup"><span data-stu-id="a86d0-137">String</span></span>|<span data-ttu-id="a86d0-138">Имя категории электронной книги.</span><span class="sxs-lookup"><span data-stu-id="a86d0-138">The name of the eBook category.</span></span>|
|<span data-ttu-id="a86d0-139">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="a86d0-139">lastModifiedDateTime</span></span>|<span data-ttu-id="a86d0-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a86d0-140">DateTimeOffset</span></span>|<span data-ttu-id="a86d0-141">Дата и время последнего изменения Манажедебуккатегори.</span><span class="sxs-lookup"><span data-stu-id="a86d0-141">The date and time the ManagedEBookCategory was last modified.</span></span>|



## <a name="response"></a><span data-ttu-id="a86d0-142">Отклик</span><span class="sxs-lookup"><span data-stu-id="a86d0-142">Response</span></span>
<span data-ttu-id="a86d0-143">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [манажедебуккатегори](../resources/intune-books-managedebookcategory.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="a86d0-143">If successful, this method returns a `200 OK` response code and an updated [managedEBookCategory](../resources/intune-books-managedebookcategory.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a86d0-144">Пример</span><span class="sxs-lookup"><span data-stu-id="a86d0-144">Example</span></span>

### <a name="request"></a><span data-ttu-id="a86d0-145">Запрос</span><span class="sxs-lookup"><span data-stu-id="a86d0-145">Request</span></span>
<span data-ttu-id="a86d0-146">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="a86d0-146">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/managedEBookCategories/{managedEBookCategoryId}
Content-type: application/json
Content-length: 102

{
  "@odata.type": "#microsoft.graph.managedEBookCategory",
  "displayName": "Display Name value"
}
```

### <a name="response"></a><span data-ttu-id="a86d0-147">Отклик</span><span class="sxs-lookup"><span data-stu-id="a86d0-147">Response</span></span>
<span data-ttu-id="a86d0-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="a86d0-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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






