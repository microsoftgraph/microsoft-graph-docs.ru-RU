---
title: Обновление Манажедебуккатегори
description: Обновление свойств объекта Манажедебуккатегори.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 91dd753ec6a40539e1b85b1aa30635a2497014ad
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42450281"
---
# <a name="update-managedebookcategory"></a><span data-ttu-id="6ae87-103">Обновление Манажедебуккатегори</span><span class="sxs-lookup"><span data-stu-id="6ae87-103">Update managedEBookCategory</span></span>

<span data-ttu-id="6ae87-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="6ae87-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="6ae87-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6ae87-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="6ae87-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="6ae87-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6ae87-107">Обновление свойств объекта [манажедебуккатегори](../resources/intune-books-managedebookcategory.md) .</span><span class="sxs-lookup"><span data-stu-id="6ae87-107">Update the properties of a [managedEBookCategory](../resources/intune-books-managedebookcategory.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="6ae87-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="6ae87-108">Prerequisites</span></span>
<span data-ttu-id="6ae87-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6ae87-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6ae87-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="6ae87-111">Permission type</span></span>|<span data-ttu-id="6ae87-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="6ae87-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6ae87-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="6ae87-113">Delegated (work or school account)</span></span>|<span data-ttu-id="6ae87-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6ae87-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="6ae87-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="6ae87-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6ae87-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6ae87-116">Not supported.</span></span>|
|<span data-ttu-id="6ae87-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="6ae87-117">Application</span></span>|<span data-ttu-id="6ae87-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6ae87-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="6ae87-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="6ae87-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/managedEBookCategories/{managedEBookCategoryId}
PATCH /deviceAppManagement/managedEBooks/{managedEBookId}/categories/{managedEBookCategoryId}
```

## <a name="request-headers"></a><span data-ttu-id="6ae87-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="6ae87-120">Request headers</span></span>
|<span data-ttu-id="6ae87-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="6ae87-121">Header</span></span>|<span data-ttu-id="6ae87-122">Значение</span><span class="sxs-lookup"><span data-stu-id="6ae87-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="6ae87-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="6ae87-123">Authorization</span></span>|<span data-ttu-id="6ae87-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="6ae87-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="6ae87-125">Accept</span><span class="sxs-lookup"><span data-stu-id="6ae87-125">Accept</span></span>|<span data-ttu-id="6ae87-126">application/json</span><span class="sxs-lookup"><span data-stu-id="6ae87-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="6ae87-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="6ae87-127">Request body</span></span>
<span data-ttu-id="6ae87-128">В тексте запроса добавьте представление объекта [манажедебуккатегори](../resources/intune-books-managedebookcategory.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="6ae87-128">In the request body, supply a JSON representation for the [managedEBookCategory](../resources/intune-books-managedebookcategory.md) object.</span></span>

<span data-ttu-id="6ae87-129">В следующей таблице приведены свойства, необходимые при создании [манажедебуккатегори](../resources/intune-books-managedebookcategory.md).</span><span class="sxs-lookup"><span data-stu-id="6ae87-129">The following table shows the properties that are required when you create the [managedEBookCategory](../resources/intune-books-managedebookcategory.md).</span></span>

|<span data-ttu-id="6ae87-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="6ae87-130">Property</span></span>|<span data-ttu-id="6ae87-131">Тип</span><span class="sxs-lookup"><span data-stu-id="6ae87-131">Type</span></span>|<span data-ttu-id="6ae87-132">Описание</span><span class="sxs-lookup"><span data-stu-id="6ae87-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6ae87-133">id</span><span class="sxs-lookup"><span data-stu-id="6ae87-133">id</span></span>|<span data-ttu-id="6ae87-134">String</span><span class="sxs-lookup"><span data-stu-id="6ae87-134">String</span></span>|<span data-ttu-id="6ae87-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="6ae87-135">The key of the entity.</span></span>|
|<span data-ttu-id="6ae87-136">displayName</span><span class="sxs-lookup"><span data-stu-id="6ae87-136">displayName</span></span>|<span data-ttu-id="6ae87-137">Строка</span><span class="sxs-lookup"><span data-stu-id="6ae87-137">String</span></span>|<span data-ttu-id="6ae87-138">Имя категории электронной книги.</span><span class="sxs-lookup"><span data-stu-id="6ae87-138">The name of the eBook category.</span></span>|
|<span data-ttu-id="6ae87-139">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="6ae87-139">lastModifiedDateTime</span></span>|<span data-ttu-id="6ae87-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6ae87-140">DateTimeOffset</span></span>|<span data-ttu-id="6ae87-141">Дата и время последнего изменения Манажедебуккатегори.</span><span class="sxs-lookup"><span data-stu-id="6ae87-141">The date and time the ManagedEBookCategory was last modified.</span></span>|



## <a name="response"></a><span data-ttu-id="6ae87-142">Отклик</span><span class="sxs-lookup"><span data-stu-id="6ae87-142">Response</span></span>
<span data-ttu-id="6ae87-143">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [манажедебуккатегори](../resources/intune-books-managedebookcategory.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="6ae87-143">If successful, this method returns a `200 OK` response code and an updated [managedEBookCategory](../resources/intune-books-managedebookcategory.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6ae87-144">Пример</span><span class="sxs-lookup"><span data-stu-id="6ae87-144">Example</span></span>

### <a name="request"></a><span data-ttu-id="6ae87-145">Запрос</span><span class="sxs-lookup"><span data-stu-id="6ae87-145">Request</span></span>
<span data-ttu-id="6ae87-146">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="6ae87-146">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/managedEBookCategories/{managedEBookCategoryId}
Content-type: application/json
Content-length: 102

{
  "@odata.type": "#microsoft.graph.managedEBookCategory",
  "displayName": "Display Name value"
}
```

### <a name="response"></a><span data-ttu-id="6ae87-147">Отклик</span><span class="sxs-lookup"><span data-stu-id="6ae87-147">Response</span></span>
<span data-ttu-id="6ae87-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="6ae87-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





