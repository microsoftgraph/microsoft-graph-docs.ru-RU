---
title: Тип ресурса termsAndConditionsAcceptanceStatus
description: C) политики данным пользователем. Чтобы получить доступ к корпоративному порталу, пользователям нужно принять последнюю версию условий.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 1c66b7ba799def675ab3b74ad2ea9b8ce2f7ec22
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27961080"
---
# <a name="termsandconditionsacceptancestatus-resource-type"></a><span data-ttu-id="8388e-104">Тип ресурса termsAndConditionsAcceptanceStatus</span><span class="sxs-lookup"><span data-stu-id="8388e-104">termsAndConditionsAcceptanceStatus resource type</span></span>

> <span data-ttu-id="8388e-105">**Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="8388e-105">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="8388e-106">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8388e-106">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="8388e-107">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="8388e-107">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="8388e-108">Объект termsAndConditionsAcceptanceStatus представляет состояние принятия определенной политики условий для заданного пользователя.</span><span class="sxs-lookup"><span data-stu-id="8388e-108">A termsAndConditionsAcceptanceStatus entity represents the acceptance status of a given Terms and Conditions (T&C) policy by a given user.</span></span> <span data-ttu-id="8388e-109">Чтобы получить доступ к корпоративному порталу, пользователям нужно принять последнюю версию условий.</span><span class="sxs-lookup"><span data-stu-id="8388e-109">Users must accept the most up-to-date version of the terms in order to retain access to the Company Portal.</span></span>
## <a name="methods"></a><span data-ttu-id="8388e-110">Методы</span><span class="sxs-lookup"><span data-stu-id="8388e-110">Methods</span></span>
|<span data-ttu-id="8388e-111">Метод</span><span class="sxs-lookup"><span data-stu-id="8388e-111">Method</span></span>|<span data-ttu-id="8388e-112">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="8388e-112">Return Type</span></span>|<span data-ttu-id="8388e-113">Описание</span><span class="sxs-lookup"><span data-stu-id="8388e-113">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="8388e-114">Список termsAndConditionsAcceptanceStatuses</span><span class="sxs-lookup"><span data-stu-id="8388e-114">List termsAndConditionsAcceptanceStatuses</span></span>](../api/intune-companyterms-termsandconditionsacceptancestatus-list.md)|<span data-ttu-id="8388e-115">Коллекция [termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md)</span><span class="sxs-lookup"><span data-stu-id="8388e-115">[termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md) collection</span></span>|<span data-ttu-id="8388e-116">Список свойств и связей объектов [termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md).</span><span class="sxs-lookup"><span data-stu-id="8388e-116">List properties and relationships of the [termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md) objects.</span></span>|
|[<span data-ttu-id="8388e-117">Получение объекта termsAndConditionsAcceptanceStatus</span><span class="sxs-lookup"><span data-stu-id="8388e-117">Get termsAndConditionsAcceptanceStatus</span></span>](../api/intune-companyterms-termsandconditionsacceptancestatus-get.md)|[<span data-ttu-id="8388e-118">termsAndConditionsAcceptanceStatus</span><span class="sxs-lookup"><span data-stu-id="8388e-118">termsAndConditionsAcceptanceStatus</span></span>](../resources/intune-companyterms-termsandconditionsacceptancestatus.md)|<span data-ttu-id="8388e-119">Чтение свойств и связей объекта [termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md).</span><span class="sxs-lookup"><span data-stu-id="8388e-119">Read properties and relationships of the [termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md) object.</span></span>|
|[<span data-ttu-id="8388e-120">Создание объекта termsAndConditionsAcceptanceStatus</span><span class="sxs-lookup"><span data-stu-id="8388e-120">Create termsAndConditionsAcceptanceStatus</span></span>](../api/intune-companyterms-termsandconditionsacceptancestatus-create.md)|[<span data-ttu-id="8388e-121">termsAndConditionsAcceptanceStatus</span><span class="sxs-lookup"><span data-stu-id="8388e-121">termsAndConditionsAcceptanceStatus</span></span>](../resources/intune-companyterms-termsandconditionsacceptancestatus.md)|<span data-ttu-id="8388e-122">Создание объекта [termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md).</span><span class="sxs-lookup"><span data-stu-id="8388e-122">Create a new [termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md) object.</span></span>|
|[<span data-ttu-id="8388e-123">Удаление объекта termsAndConditionsAcceptanceStatus</span><span class="sxs-lookup"><span data-stu-id="8388e-123">Delete termsAndConditionsAcceptanceStatus</span></span>](../api/intune-companyterms-termsandconditionsacceptancestatus-delete.md)|<span data-ttu-id="8388e-124">Нет</span><span class="sxs-lookup"><span data-stu-id="8388e-124">None</span></span>|<span data-ttu-id="8388e-125">Удаляет объект [termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md).</span><span class="sxs-lookup"><span data-stu-id="8388e-125">Deletes a [termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md).</span></span>|
|[<span data-ttu-id="8388e-126">Обновление объекта termsAndConditionsAcceptanceStatus</span><span class="sxs-lookup"><span data-stu-id="8388e-126">Update termsAndConditionsAcceptanceStatus</span></span>](../api/intune-companyterms-termsandconditionsacceptancestatus-update.md)|[<span data-ttu-id="8388e-127">termsAndConditionsAcceptanceStatus</span><span class="sxs-lookup"><span data-stu-id="8388e-127">termsAndConditionsAcceptanceStatus</span></span>](../resources/intune-companyterms-termsandconditionsacceptancestatus.md)|<span data-ttu-id="8388e-128">Обновление свойств объекта [termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md).</span><span class="sxs-lookup"><span data-stu-id="8388e-128">Update the properties of a [termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="8388e-129">Свойства</span><span class="sxs-lookup"><span data-stu-id="8388e-129">Properties</span></span>
|<span data-ttu-id="8388e-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="8388e-130">Property</span></span>|<span data-ttu-id="8388e-131">Тип</span><span class="sxs-lookup"><span data-stu-id="8388e-131">Type</span></span>|<span data-ttu-id="8388e-132">Описание</span><span class="sxs-lookup"><span data-stu-id="8388e-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8388e-133">id</span><span class="sxs-lookup"><span data-stu-id="8388e-133">id</span></span>|<span data-ttu-id="8388e-134">String</span><span class="sxs-lookup"><span data-stu-id="8388e-134">String</span></span>|<span data-ttu-id="8388e-135">Уникальный идентификатор объекта.</span><span class="sxs-lookup"><span data-stu-id="8388e-135">Unique identifier of the entity.</span></span>|
|<span data-ttu-id="8388e-136">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="8388e-136">userDisplayName</span></span>|<span data-ttu-id="8388e-137">String</span><span class="sxs-lookup"><span data-stu-id="8388e-137">String</span></span>|<span data-ttu-id="8388e-138">Отображает имя пользователя, чье принятие представлено объектом.</span><span class="sxs-lookup"><span data-stu-id="8388e-138">Display name of the user whose acceptance the entity represents.</span></span>|
|<span data-ttu-id="8388e-139">acceptedVersion</span><span class="sxs-lookup"><span data-stu-id="8388e-139">acceptedVersion</span></span>|<span data-ttu-id="8388e-140">Int32</span><span class="sxs-lookup"><span data-stu-id="8388e-140">Int32</span></span>|<span data-ttu-id="8388e-141">Номер последней версии условий, принятых пользователем.</span><span class="sxs-lookup"><span data-stu-id="8388e-141">Most recent version number of the T&C accepted by the user.</span></span>|
|<span data-ttu-id="8388e-142">acceptedDateTime</span><span class="sxs-lookup"><span data-stu-id="8388e-142">acceptedDateTime</span></span>|<span data-ttu-id="8388e-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8388e-143">DateTimeOffset</span></span>|<span data-ttu-id="8388e-144">Дата и время последнего принятия условий пользователем.</span><span class="sxs-lookup"><span data-stu-id="8388e-144">DateTime when the terms were last accepted by the user.</span></span>|

## <a name="relationships"></a><span data-ttu-id="8388e-145">Связи</span><span class="sxs-lookup"><span data-stu-id="8388e-145">Relationships</span></span>
|<span data-ttu-id="8388e-146">Связь</span><span class="sxs-lookup"><span data-stu-id="8388e-146">Relationship</span></span>|<span data-ttu-id="8388e-147">Тип</span><span class="sxs-lookup"><span data-stu-id="8388e-147">Type</span></span>|<span data-ttu-id="8388e-148">Описание</span><span class="sxs-lookup"><span data-stu-id="8388e-148">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8388e-149">termsAndConditions</span><span class="sxs-lookup"><span data-stu-id="8388e-149">termsAndConditions</span></span>|[<span data-ttu-id="8388e-150">termsAndConditions</span><span class="sxs-lookup"><span data-stu-id="8388e-150">termsAndConditions</span></span>](../resources/intune-companyterms-termsandconditions.md)|<span data-ttu-id="8388e-151">Ссылка для перехода к назначенным условиям.</span><span class="sxs-lookup"><span data-stu-id="8388e-151">Navigation link to the terms and conditions that are assigned.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="8388e-152">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="8388e-152">JSON Representation</span></span>
<span data-ttu-id="8388e-153">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="8388e-153">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.termsAndConditionsAcceptanceStatus"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.termsAndConditionsAcceptanceStatus",
  "id": "String (identifier)",
  "userDisplayName": "String",
  "acceptedVersion": 1024,
  "acceptedDateTime": "String (timestamp)"
}
```





