---
title: Создание managedEBookCategory
description: Создайте новый объект managedEBookCategory.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: ae2fd38c576d2d85f4d07137a17e3a20be78ccff
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51133033"
---
# <a name="create-managedebookcategory"></a><span data-ttu-id="1387a-103">Создание managedEBookCategory</span><span class="sxs-lookup"><span data-stu-id="1387a-103">Create managedEBookCategory</span></span>

<span data-ttu-id="1387a-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1387a-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="1387a-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1387a-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="1387a-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="1387a-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1387a-107">Создайте новый [объект managedEBookCategory.](../resources/intune-books-managedebookcategory.md)</span><span class="sxs-lookup"><span data-stu-id="1387a-107">Create a new [managedEBookCategory](../resources/intune-books-managedebookcategory.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="1387a-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="1387a-108">Prerequisites</span></span>
<span data-ttu-id="1387a-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1387a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1387a-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="1387a-111">Permission type</span></span>|<span data-ttu-id="1387a-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="1387a-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1387a-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="1387a-113">Delegated (work or school account)</span></span>|<span data-ttu-id="1387a-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1387a-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="1387a-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="1387a-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1387a-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1387a-116">Not supported.</span></span>|
|<span data-ttu-id="1387a-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="1387a-117">Application</span></span>|<span data-ttu-id="1387a-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1387a-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="1387a-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="1387a-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/managedEBookCategories
POST /deviceAppManagement/managedEBooks/{managedEBookId}/categories
```

## <a name="request-headers"></a><span data-ttu-id="1387a-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="1387a-120">Request headers</span></span>
|<span data-ttu-id="1387a-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="1387a-121">Header</span></span>|<span data-ttu-id="1387a-122">Значение</span><span class="sxs-lookup"><span data-stu-id="1387a-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="1387a-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="1387a-123">Authorization</span></span>|<span data-ttu-id="1387a-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="1387a-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="1387a-125">Accept</span><span class="sxs-lookup"><span data-stu-id="1387a-125">Accept</span></span>|<span data-ttu-id="1387a-126">application/json</span><span class="sxs-lookup"><span data-stu-id="1387a-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="1387a-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="1387a-127">Request body</span></span>
<span data-ttu-id="1387a-128">В теле запроса поставляем представление JSON для объекта managedEBookCategory.</span><span class="sxs-lookup"><span data-stu-id="1387a-128">In the request body, supply a JSON representation for the managedEBookCategory object.</span></span>

<span data-ttu-id="1387a-129">В следующей таблице показаны свойства, необходимые при создании управляемогоEBookCategory.</span><span class="sxs-lookup"><span data-stu-id="1387a-129">The following table shows the properties that are required when you create the managedEBookCategory.</span></span>

|<span data-ttu-id="1387a-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="1387a-130">Property</span></span>|<span data-ttu-id="1387a-131">Тип</span><span class="sxs-lookup"><span data-stu-id="1387a-131">Type</span></span>|<span data-ttu-id="1387a-132">Описание</span><span class="sxs-lookup"><span data-stu-id="1387a-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1387a-133">id</span><span class="sxs-lookup"><span data-stu-id="1387a-133">id</span></span>|<span data-ttu-id="1387a-134">Строка</span><span class="sxs-lookup"><span data-stu-id="1387a-134">String</span></span>|<span data-ttu-id="1387a-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="1387a-135">The key of the entity.</span></span>|
|<span data-ttu-id="1387a-136">displayName</span><span class="sxs-lookup"><span data-stu-id="1387a-136">displayName</span></span>|<span data-ttu-id="1387a-137">Строка</span><span class="sxs-lookup"><span data-stu-id="1387a-137">String</span></span>|<span data-ttu-id="1387a-138">Имя категории электронных книг.</span><span class="sxs-lookup"><span data-stu-id="1387a-138">The name of the eBook category.</span></span>|
|<span data-ttu-id="1387a-139">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="1387a-139">lastModifiedDateTime</span></span>|<span data-ttu-id="1387a-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1387a-140">DateTimeOffset</span></span>|<span data-ttu-id="1387a-141">Дата и время последнего изменения managedEBookCategory.</span><span class="sxs-lookup"><span data-stu-id="1387a-141">The date and time the ManagedEBookCategory was last modified.</span></span>|



## <a name="response"></a><span data-ttu-id="1387a-142">Отклик</span><span class="sxs-lookup"><span data-stu-id="1387a-142">Response</span></span>
<span data-ttu-id="1387a-143">В случае успешной работы этот метод возвращает код ответа и управляемый `201 Created` [объектEBookCategory](../resources/intune-books-managedebookcategory.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="1387a-143">If successful, this method returns a `201 Created` response code and a [managedEBookCategory](../resources/intune-books-managedebookcategory.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1387a-144">Пример</span><span class="sxs-lookup"><span data-stu-id="1387a-144">Example</span></span>

### <a name="request"></a><span data-ttu-id="1387a-145">Запрос</span><span class="sxs-lookup"><span data-stu-id="1387a-145">Request</span></span>
<span data-ttu-id="1387a-146">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="1387a-146">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/managedEBookCategories
Content-type: application/json
Content-length: 102

{
  "@odata.type": "#microsoft.graph.managedEBookCategory",
  "displayName": "Display Name value"
}
```

### <a name="response"></a><span data-ttu-id="1387a-147">Отклик</span><span class="sxs-lookup"><span data-stu-id="1387a-147">Response</span></span>
<span data-ttu-id="1387a-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="1387a-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




