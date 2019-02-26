---
title: Тип ресурса termsAndConditionsAcceptanceStatus
description: Объект termsAndConditionsAcceptanceStatus представляет состояние принятия определенной политики условий для заданного пользователя. Чтобы получить доступ к корпоративному порталу, пользователям нужно принять последнюю версию условий.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 3df5a81870729fba79519be4010c852aa6810f50
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/26/2019
ms.locfileid: "30251050"
---
# <a name="termsandconditionsacceptancestatus-resource-type"></a><span data-ttu-id="88ca1-104">Тип ресурса termsAndConditionsAcceptanceStatus</span><span class="sxs-lookup"><span data-stu-id="88ca1-104">termsAndConditionsAcceptanceStatus resource type</span></span>

> <span data-ttu-id="88ca1-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="88ca1-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="88ca1-106">Объект termsAndConditionsAcceptanceStatus представляет состояние принятия определенной политики условий для заданного пользователя.</span><span class="sxs-lookup"><span data-stu-id="88ca1-106">A termsAndConditionsAcceptanceStatus entity represents the acceptance status of a given Terms and Conditions (T&C) policy by a given user.</span></span> <span data-ttu-id="88ca1-107">Чтобы получить доступ к корпоративному порталу, пользователям нужно принять последнюю версию условий.</span><span class="sxs-lookup"><span data-stu-id="88ca1-107">Users must accept the most up-to-date version of the terms in order to retain access to the Company Portal.</span></span>

## <a name="methods"></a><span data-ttu-id="88ca1-108">Методы</span><span class="sxs-lookup"><span data-stu-id="88ca1-108">Methods</span></span>
|<span data-ttu-id="88ca1-109">Метод</span><span class="sxs-lookup"><span data-stu-id="88ca1-109">Method</span></span>|<span data-ttu-id="88ca1-110">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="88ca1-110">Return Type</span></span>|<span data-ttu-id="88ca1-111">Описание</span><span class="sxs-lookup"><span data-stu-id="88ca1-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="88ca1-112">Список termsAndConditionsAcceptanceStatuses</span><span class="sxs-lookup"><span data-stu-id="88ca1-112">List termsAndConditionsAcceptanceStatuses</span></span>](../api/intune-companyterms-termsandconditionsacceptancestatus-list.md)|<span data-ttu-id="88ca1-113">Коллекция [termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md)</span><span class="sxs-lookup"><span data-stu-id="88ca1-113">[termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md) collection</span></span>|<span data-ttu-id="88ca1-114">Список свойств и связей объектов [termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md).</span><span class="sxs-lookup"><span data-stu-id="88ca1-114">List properties and relationships of the [termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md) objects.</span></span>|
|[<span data-ttu-id="88ca1-115">Получение объекта termsAndConditionsAcceptanceStatus</span><span class="sxs-lookup"><span data-stu-id="88ca1-115">Get termsAndConditionsAcceptanceStatus</span></span>](../api/intune-companyterms-termsandconditionsacceptancestatus-get.md)|<span data-ttu-id="88ca1-116">[termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md);</span><span class="sxs-lookup"><span data-stu-id="88ca1-116">[termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md)</span></span>|<span data-ttu-id="88ca1-117">Чтение свойств и связей объекта [termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md).</span><span class="sxs-lookup"><span data-stu-id="88ca1-117">Read properties and relationships of the [termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md) object.</span></span>|
|[<span data-ttu-id="88ca1-118">Создание объекта termsAndConditionsAcceptanceStatus</span><span class="sxs-lookup"><span data-stu-id="88ca1-118">Create termsAndConditionsAcceptanceStatus</span></span>](../api/intune-companyterms-termsandconditionsacceptancestatus-create.md)|<span data-ttu-id="88ca1-119">[termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md);</span><span class="sxs-lookup"><span data-stu-id="88ca1-119">[termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md)</span></span>|<span data-ttu-id="88ca1-120">Создание объекта [termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md).</span><span class="sxs-lookup"><span data-stu-id="88ca1-120">Create a new [termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md) object.</span></span>|
|[<span data-ttu-id="88ca1-121">Удаление объекта termsAndConditionsAcceptanceStatus</span><span class="sxs-lookup"><span data-stu-id="88ca1-121">Delete termsAndConditionsAcceptanceStatus</span></span>](../api/intune-companyterms-termsandconditionsacceptancestatus-delete.md)|<span data-ttu-id="88ca1-122">Нет</span><span class="sxs-lookup"><span data-stu-id="88ca1-122">None</span></span>|<span data-ttu-id="88ca1-123">Удаляет объект [termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md).</span><span class="sxs-lookup"><span data-stu-id="88ca1-123">Deletes a [termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md).</span></span>|
|[<span data-ttu-id="88ca1-124">Обновление объекта termsAndConditionsAcceptanceStatus</span><span class="sxs-lookup"><span data-stu-id="88ca1-124">Update termsAndConditionsAcceptanceStatus</span></span>](../api/intune-companyterms-termsandconditionsacceptancestatus-update.md)|[<span data-ttu-id="88ca1-125">termsAndConditionsAcceptanceStatus</span><span class="sxs-lookup"><span data-stu-id="88ca1-125">termsAndConditionsAcceptanceStatus</span></span>](../resources/intune-companyterms-termsandconditionsacceptancestatus.md)|<span data-ttu-id="88ca1-126">Обновление свойств объекта [termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md).</span><span class="sxs-lookup"><span data-stu-id="88ca1-126">Update the properties of a [termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="88ca1-127">Свойства</span><span class="sxs-lookup"><span data-stu-id="88ca1-127">Properties</span></span>
|<span data-ttu-id="88ca1-128">Свойство</span><span class="sxs-lookup"><span data-stu-id="88ca1-128">Property</span></span>|<span data-ttu-id="88ca1-129">Тип</span><span class="sxs-lookup"><span data-stu-id="88ca1-129">Type</span></span>|<span data-ttu-id="88ca1-130">Описание</span><span class="sxs-lookup"><span data-stu-id="88ca1-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="88ca1-131">id</span><span class="sxs-lookup"><span data-stu-id="88ca1-131">id</span></span>|<span data-ttu-id="88ca1-132">Строка</span><span class="sxs-lookup"><span data-stu-id="88ca1-132">String</span></span>|<span data-ttu-id="88ca1-133">Уникальный идентификатор объекта.</span><span class="sxs-lookup"><span data-stu-id="88ca1-133">Unique identifier of the entity.</span></span>|
|<span data-ttu-id="88ca1-134">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="88ca1-134">userDisplayName</span></span>|<span data-ttu-id="88ca1-135">String</span><span class="sxs-lookup"><span data-stu-id="88ca1-135">String</span></span>|<span data-ttu-id="88ca1-136">Отображает имя пользователя, чье принятие представлено объектом.</span><span class="sxs-lookup"><span data-stu-id="88ca1-136">Display name of the user whose acceptance the entity represents.</span></span>|
|<span data-ttu-id="88ca1-137">acceptedVersion</span><span class="sxs-lookup"><span data-stu-id="88ca1-137">acceptedVersion</span></span>|<span data-ttu-id="88ca1-138">Int32</span><span class="sxs-lookup"><span data-stu-id="88ca1-138">Int32</span></span>|<span data-ttu-id="88ca1-139">Номер последней версии условий, принятых пользователем.</span><span class="sxs-lookup"><span data-stu-id="88ca1-139">Most recent version number of the T&C accepted by the user.</span></span>|
|<span data-ttu-id="88ca1-140">acceptedDateTime</span><span class="sxs-lookup"><span data-stu-id="88ca1-140">acceptedDateTime</span></span>|<span data-ttu-id="88ca1-141">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="88ca1-141">DateTimeOffset</span></span>|<span data-ttu-id="88ca1-142">Дата и время последнего принятия условий пользователем.</span><span class="sxs-lookup"><span data-stu-id="88ca1-142">DateTime when the terms were last accepted by the user.</span></span>|

## <a name="relationships"></a><span data-ttu-id="88ca1-143">Связи</span><span class="sxs-lookup"><span data-stu-id="88ca1-143">Relationships</span></span>
|<span data-ttu-id="88ca1-144">Отношение</span><span class="sxs-lookup"><span data-stu-id="88ca1-144">Relationship</span></span>|<span data-ttu-id="88ca1-145">Тип</span><span class="sxs-lookup"><span data-stu-id="88ca1-145">Type</span></span>|<span data-ttu-id="88ca1-146">Описание</span><span class="sxs-lookup"><span data-stu-id="88ca1-146">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="88ca1-147">termsAndConditions</span><span class="sxs-lookup"><span data-stu-id="88ca1-147">termsAndConditions</span></span>|[<span data-ttu-id="88ca1-148">termsAndConditions</span><span class="sxs-lookup"><span data-stu-id="88ca1-148">termsAndConditions</span></span>](../resources/intune-companyterms-termsandconditions.md)|<span data-ttu-id="88ca1-149">Ссылка для перехода к назначенным условиям.</span><span class="sxs-lookup"><span data-stu-id="88ca1-149">Navigation link to the terms and conditions that are assigned.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="88ca1-150">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="88ca1-150">JSON Representation</span></span>
<span data-ttu-id="88ca1-151">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="88ca1-151">Here is a JSON representation of the resource.</span></span>
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



