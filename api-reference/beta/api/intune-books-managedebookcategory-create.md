---
title: Создание Манажедебуккатегори
description: Создание нового объекта Манажедебуккатегори.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: b3d59e4b8e31a894c30237b96ddb524478a420f4
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43392227"
---
# <a name="create-managedebookcategory"></a><span data-ttu-id="b355d-103">Создание Манажедебуккатегори</span><span class="sxs-lookup"><span data-stu-id="b355d-103">Create managedEBookCategory</span></span>

<span data-ttu-id="b355d-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b355d-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="b355d-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b355d-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b355d-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="b355d-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b355d-107">Создание нового объекта [манажедебуккатегори](../resources/intune-books-managedebookcategory.md) .</span><span class="sxs-lookup"><span data-stu-id="b355d-107">Create a new [managedEBookCategory](../resources/intune-books-managedebookcategory.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="b355d-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="b355d-108">Prerequisites</span></span>
<span data-ttu-id="b355d-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b355d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b355d-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="b355d-111">Permission type</span></span>|<span data-ttu-id="b355d-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="b355d-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b355d-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="b355d-113">Delegated (work or school account)</span></span>|<span data-ttu-id="b355d-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b355d-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="b355d-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="b355d-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b355d-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b355d-116">Not supported.</span></span>|
|<span data-ttu-id="b355d-117">Для приложения</span><span class="sxs-lookup"><span data-stu-id="b355d-117">Application</span></span>|<span data-ttu-id="b355d-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b355d-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="b355d-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="b355d-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/managedEBookCategories
POST /deviceAppManagement/managedEBooks/{managedEBookId}/categories
```

## <a name="request-headers"></a><span data-ttu-id="b355d-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="b355d-120">Request headers</span></span>
|<span data-ttu-id="b355d-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="b355d-121">Header</span></span>|<span data-ttu-id="b355d-122">Значение</span><span class="sxs-lookup"><span data-stu-id="b355d-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b355d-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="b355d-123">Authorization</span></span>|<span data-ttu-id="b355d-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="b355d-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b355d-125">Accept</span><span class="sxs-lookup"><span data-stu-id="b355d-125">Accept</span></span>|<span data-ttu-id="b355d-126">application/json</span><span class="sxs-lookup"><span data-stu-id="b355d-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b355d-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="b355d-127">Request body</span></span>
<span data-ttu-id="b355d-128">В тексте запроса добавьте представление объекта Манажедебуккатегори в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="b355d-128">In the request body, supply a JSON representation for the managedEBookCategory object.</span></span>

<span data-ttu-id="b355d-129">В следующей таблице приведены свойства, необходимые при создании Манажедебуккатегори.</span><span class="sxs-lookup"><span data-stu-id="b355d-129">The following table shows the properties that are required when you create the managedEBookCategory.</span></span>

|<span data-ttu-id="b355d-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="b355d-130">Property</span></span>|<span data-ttu-id="b355d-131">Тип</span><span class="sxs-lookup"><span data-stu-id="b355d-131">Type</span></span>|<span data-ttu-id="b355d-132">Описание</span><span class="sxs-lookup"><span data-stu-id="b355d-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b355d-133">id</span><span class="sxs-lookup"><span data-stu-id="b355d-133">id</span></span>|<span data-ttu-id="b355d-134">String</span><span class="sxs-lookup"><span data-stu-id="b355d-134">String</span></span>|<span data-ttu-id="b355d-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="b355d-135">The key of the entity.</span></span>|
|<span data-ttu-id="b355d-136">displayName</span><span class="sxs-lookup"><span data-stu-id="b355d-136">displayName</span></span>|<span data-ttu-id="b355d-137">Строка</span><span class="sxs-lookup"><span data-stu-id="b355d-137">String</span></span>|<span data-ttu-id="b355d-138">Имя категории электронной книги.</span><span class="sxs-lookup"><span data-stu-id="b355d-138">The name of the eBook category.</span></span>|
|<span data-ttu-id="b355d-139">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="b355d-139">lastModifiedDateTime</span></span>|<span data-ttu-id="b355d-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b355d-140">DateTimeOffset</span></span>|<span data-ttu-id="b355d-141">Дата и время последнего изменения Манажедебуккатегори.</span><span class="sxs-lookup"><span data-stu-id="b355d-141">The date and time the ManagedEBookCategory was last modified.</span></span>|



## <a name="response"></a><span data-ttu-id="b355d-142">Отклик</span><span class="sxs-lookup"><span data-stu-id="b355d-142">Response</span></span>
<span data-ttu-id="b355d-143">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [манажедебуккатегори](../resources/intune-books-managedebookcategory.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="b355d-143">If successful, this method returns a `201 Created` response code and a [managedEBookCategory](../resources/intune-books-managedebookcategory.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b355d-144">Пример</span><span class="sxs-lookup"><span data-stu-id="b355d-144">Example</span></span>

### <a name="request"></a><span data-ttu-id="b355d-145">Запрос</span><span class="sxs-lookup"><span data-stu-id="b355d-145">Request</span></span>
<span data-ttu-id="b355d-146">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="b355d-146">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/managedEBookCategories
Content-type: application/json
Content-length: 102

{
  "@odata.type": "#microsoft.graph.managedEBookCategory",
  "displayName": "Display Name value"
}
```

### <a name="response"></a><span data-ttu-id="b355d-147">Отклик</span><span class="sxs-lookup"><span data-stu-id="b355d-147">Response</span></span>
<span data-ttu-id="b355d-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="b355d-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



