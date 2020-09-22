---
title: Создание Манажедебуккатегори
description: Создание нового объекта Манажедебуккатегори.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 5fa61c7d0b75a510f9f1f4a5c752257ee8f56d09
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "47975509"
---
# <a name="create-managedebookcategory"></a><span data-ttu-id="1d4dd-103">Создание Манажедебуккатегори</span><span class="sxs-lookup"><span data-stu-id="1d4dd-103">Create managedEBookCategory</span></span>

<span data-ttu-id="1d4dd-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1d4dd-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="1d4dd-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1d4dd-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="1d4dd-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="1d4dd-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1d4dd-107">Создание нового объекта [манажедебуккатегори](../resources/intune-books-managedebookcategory.md) .</span><span class="sxs-lookup"><span data-stu-id="1d4dd-107">Create a new [managedEBookCategory](../resources/intune-books-managedebookcategory.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="1d4dd-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="1d4dd-108">Prerequisites</span></span>
<span data-ttu-id="1d4dd-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1d4dd-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1d4dd-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="1d4dd-111">Permission type</span></span>|<span data-ttu-id="1d4dd-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="1d4dd-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1d4dd-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="1d4dd-113">Delegated (work or school account)</span></span>|<span data-ttu-id="1d4dd-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1d4dd-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="1d4dd-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="1d4dd-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1d4dd-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1d4dd-116">Not supported.</span></span>|
|<span data-ttu-id="1d4dd-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="1d4dd-117">Application</span></span>|<span data-ttu-id="1d4dd-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1d4dd-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="1d4dd-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="1d4dd-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/managedEBookCategories
POST /deviceAppManagement/managedEBooks/{managedEBookId}/categories
```

## <a name="request-headers"></a><span data-ttu-id="1d4dd-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="1d4dd-120">Request headers</span></span>
|<span data-ttu-id="1d4dd-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="1d4dd-121">Header</span></span>|<span data-ttu-id="1d4dd-122">Значение</span><span class="sxs-lookup"><span data-stu-id="1d4dd-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="1d4dd-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="1d4dd-123">Authorization</span></span>|<span data-ttu-id="1d4dd-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="1d4dd-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="1d4dd-125">Accept</span><span class="sxs-lookup"><span data-stu-id="1d4dd-125">Accept</span></span>|<span data-ttu-id="1d4dd-126">application/json</span><span class="sxs-lookup"><span data-stu-id="1d4dd-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="1d4dd-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="1d4dd-127">Request body</span></span>
<span data-ttu-id="1d4dd-128">В тексте запроса добавьте представление объекта Манажедебуккатегори в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="1d4dd-128">In the request body, supply a JSON representation for the managedEBookCategory object.</span></span>

<span data-ttu-id="1d4dd-129">В следующей таблице приведены свойства, необходимые при создании Манажедебуккатегори.</span><span class="sxs-lookup"><span data-stu-id="1d4dd-129">The following table shows the properties that are required when you create the managedEBookCategory.</span></span>

|<span data-ttu-id="1d4dd-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="1d4dd-130">Property</span></span>|<span data-ttu-id="1d4dd-131">Тип</span><span class="sxs-lookup"><span data-stu-id="1d4dd-131">Type</span></span>|<span data-ttu-id="1d4dd-132">Описание</span><span class="sxs-lookup"><span data-stu-id="1d4dd-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1d4dd-133">id</span><span class="sxs-lookup"><span data-stu-id="1d4dd-133">id</span></span>|<span data-ttu-id="1d4dd-134">String</span><span class="sxs-lookup"><span data-stu-id="1d4dd-134">String</span></span>|<span data-ttu-id="1d4dd-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="1d4dd-135">The key of the entity.</span></span>|
|<span data-ttu-id="1d4dd-136">displayName</span><span class="sxs-lookup"><span data-stu-id="1d4dd-136">displayName</span></span>|<span data-ttu-id="1d4dd-137">String</span><span class="sxs-lookup"><span data-stu-id="1d4dd-137">String</span></span>|<span data-ttu-id="1d4dd-138">Имя категории электронной книги.</span><span class="sxs-lookup"><span data-stu-id="1d4dd-138">The name of the eBook category.</span></span>|
|<span data-ttu-id="1d4dd-139">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="1d4dd-139">lastModifiedDateTime</span></span>|<span data-ttu-id="1d4dd-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1d4dd-140">DateTimeOffset</span></span>|<span data-ttu-id="1d4dd-141">Дата и время последнего изменения Манажедебуккатегори.</span><span class="sxs-lookup"><span data-stu-id="1d4dd-141">The date and time the ManagedEBookCategory was last modified.</span></span>|



## <a name="response"></a><span data-ttu-id="1d4dd-142">Отклик</span><span class="sxs-lookup"><span data-stu-id="1d4dd-142">Response</span></span>
<span data-ttu-id="1d4dd-143">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [манажедебуккатегори](../resources/intune-books-managedebookcategory.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="1d4dd-143">If successful, this method returns a `201 Created` response code and a [managedEBookCategory](../resources/intune-books-managedebookcategory.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1d4dd-144">Пример</span><span class="sxs-lookup"><span data-stu-id="1d4dd-144">Example</span></span>

### <a name="request"></a><span data-ttu-id="1d4dd-145">Запрос</span><span class="sxs-lookup"><span data-stu-id="1d4dd-145">Request</span></span>
<span data-ttu-id="1d4dd-146">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="1d4dd-146">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/managedEBookCategories
Content-type: application/json
Content-length: 102

{
  "@odata.type": "#microsoft.graph.managedEBookCategory",
  "displayName": "Display Name value"
}
```

### <a name="response"></a><span data-ttu-id="1d4dd-147">Отклик</span><span class="sxs-lookup"><span data-stu-id="1d4dd-147">Response</span></span>
<span data-ttu-id="1d4dd-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="1d4dd-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 215

{
  "@odata.type": "#microsoft.graph.managedEBookCategory",
  "id": "3c71fb14-fb14-3c71-14fb-713c14fb713c",
  "displayName": "Display Name value",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00"
}
```






