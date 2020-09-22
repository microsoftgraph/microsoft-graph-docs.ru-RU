---
title: Тип ресурса договора
description: Представляет настраиваемое соглашение об использовании клиента, которое создается и управляется с помощью Azure Active Directory (Azure AD).
localization_priority: Normal
doc_type: resourcePageType
ms.prod: microsoft-identity-platform
author: raprakasMSFT
ms.openlocfilehash: a6b987e36769102ee32eeb9509554f8e78fed9d0
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48067512"
---
# <a name="agreement-resource-type"></a><span data-ttu-id="6f053-103">Тип ресурса договора</span><span class="sxs-lookup"><span data-stu-id="6f053-103">agreement resource type</span></span>

<span data-ttu-id="6f053-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6f053-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6f053-105">Представляет настраиваемое соглашение об использовании клиента, которое создается и управляется с помощью Azure Active Directory (Azure AD).</span><span class="sxs-lookup"><span data-stu-id="6f053-105">Represents a tenant's customizable terms of use agreement that is created and managed with Azure Active Directory (Azure AD).</span></span> <span data-ttu-id="6f053-106">Вы можете использовать следующие методы для создания и управления [условиями использования функции Azure Active Directory](/azure/active-directory/active-directory-tou) в соответствии со сценарием.</span><span class="sxs-lookup"><span data-stu-id="6f053-106">You can use the following methods to create and manage the [Azure Active Directory Terms of Use feature](/azure/active-directory/active-directory-tou) according to your scenario.</span></span>

## <a name="methods"></a><span data-ttu-id="6f053-107">Методы</span><span class="sxs-lookup"><span data-stu-id="6f053-107">Methods</span></span>

| <span data-ttu-id="6f053-108">Метод</span><span class="sxs-lookup"><span data-stu-id="6f053-108">Method</span></span>       | <span data-ttu-id="6f053-109">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="6f053-109">Return Type</span></span> | <span data-ttu-id="6f053-110">Описание</span><span class="sxs-lookup"><span data-stu-id="6f053-110">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="6f053-111">Создание договоров</span><span class="sxs-lookup"><span data-stu-id="6f053-111">Create agreements</span></span>](../api/agreement-post-agreements.md) | [<span data-ttu-id="6f053-112">Корпоратив</span><span class="sxs-lookup"><span data-stu-id="6f053-112">agreement</span></span>](agreement.md) | <span data-ttu-id="6f053-113">Создание нового соглашения путем публикации в коллекции договоров.</span><span class="sxs-lookup"><span data-stu-id="6f053-113">Create a new agreement by posting to the agreement collection.</span></span> |
| [<span data-ttu-id="6f053-114">Список соглашений</span><span class="sxs-lookup"><span data-stu-id="6f053-114">List agreements</span></span>](../api/agreement-list.md) | <span data-ttu-id="6f053-115">Коллекция [договоров](agreement.md)</span><span class="sxs-lookup"><span data-stu-id="6f053-115">[agreement](agreement.md) collection</span></span> | <span data-ttu-id="6f053-116">Получение коллекции объектов Agreement.</span><span class="sxs-lookup"><span data-stu-id="6f053-116">Get an agreement object collection.</span></span> |
| [<span data-ttu-id="6f053-117">Получение соглашения</span><span class="sxs-lookup"><span data-stu-id="6f053-117">Get agreement</span></span>](../api/agreement-get.md) | [<span data-ttu-id="6f053-118">Корпоратив</span><span class="sxs-lookup"><span data-stu-id="6f053-118">agreement</span></span>](agreement.md) | <span data-ttu-id="6f053-119">Чтение свойств и связей объекта Agreement.</span><span class="sxs-lookup"><span data-stu-id="6f053-119">Read properties and relationships of an agreement object.</span></span> |
| [<span data-ttu-id="6f053-120">Обновление соглашения</span><span class="sxs-lookup"><span data-stu-id="6f053-120">Update agreement</span></span>](../api/agreement-update.md) | [<span data-ttu-id="6f053-121">Корпоратив</span><span class="sxs-lookup"><span data-stu-id="6f053-121">agreement</span></span>](agreement.md) | <span data-ttu-id="6f053-122">Обновление объекта договора.</span><span class="sxs-lookup"><span data-stu-id="6f053-122">Update an agreement object.</span></span> |
| [<span data-ttu-id="6f053-123">Удаление соглашения</span><span class="sxs-lookup"><span data-stu-id="6f053-123">Delete agreement</span></span>](../api/agreement-delete.md) | <span data-ttu-id="6f053-124">Нет</span><span class="sxs-lookup"><span data-stu-id="6f053-124">None</span></span> | <span data-ttu-id="6f053-125">Удаление объекта соглашения.</span><span class="sxs-lookup"><span data-stu-id="6f053-125">Delete an agreement object.</span></span> |
<!--
| [Create agreementFile](../api/agreement-post-files.md) | [agreementFile](agreementfile.md) | Create a new agreementFile by posting to the files collection. |
| [List files](../api/agreement-list-files.md) | [agreementFile](agreementfile.md) collection | Get an agreementFile object collection. |
-->

## <a name="properties"></a><span data-ttu-id="6f053-126">Свойства</span><span class="sxs-lookup"><span data-stu-id="6f053-126">Properties</span></span>
| <span data-ttu-id="6f053-127">Свойство</span><span class="sxs-lookup"><span data-stu-id="6f053-127">Property</span></span>     | <span data-ttu-id="6f053-128">Тип</span><span class="sxs-lookup"><span data-stu-id="6f053-128">Type</span></span>        | <span data-ttu-id="6f053-129">Описание</span><span class="sxs-lookup"><span data-stu-id="6f053-129">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="6f053-130">displayName</span><span class="sxs-lookup"><span data-stu-id="6f053-130">displayName</span></span>|<span data-ttu-id="6f053-131">String</span><span class="sxs-lookup"><span data-stu-id="6f053-131">String</span></span>|<span data-ttu-id="6f053-132">Отображаемое имя соглашения.</span><span class="sxs-lookup"><span data-stu-id="6f053-132">Display name of the agreement.</span></span> <span data-ttu-id="6f053-133">Отображаемое имя используется для внутренней трассировки соглашения, но оно не отображается для конечных пользователей, которые просматривают соглашение.</span><span class="sxs-lookup"><span data-stu-id="6f053-133">The display name is used for internal tracking of the agreement but is not shown to end users who view the agreement.</span></span>|
|<span data-ttu-id="6f053-134">id</span><span class="sxs-lookup"><span data-stu-id="6f053-134">id</span></span>|<span data-ttu-id="6f053-135">String</span><span class="sxs-lookup"><span data-stu-id="6f053-135">String</span></span>| <span data-ttu-id="6f053-136">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="6f053-136">Read-only.</span></span>|
|<span data-ttu-id="6f053-137">isPerDeviceAcceptanceRequired</span><span class="sxs-lookup"><span data-stu-id="6f053-137">isPerDeviceAcceptanceRequired</span></span>|<span data-ttu-id="6f053-138">Boolean</span><span class="sxs-lookup"><span data-stu-id="6f053-138">Boolean</span></span>|<span data-ttu-id="6f053-139">Этот параметр позволяет конечным пользователям принимать данное соглашение для всех устройств, к которым они обращаются.</span><span class="sxs-lookup"><span data-stu-id="6f053-139">This setting enables you to require end users to accept this agreement on every device that they are accessing it from.</span></span> <span data-ttu-id="6f053-140">Конечному пользователю потребуется зарегистрировать свое устройство в Azure AD, если это еще не сделано.</span><span class="sxs-lookup"><span data-stu-id="6f053-140">The end user will be required to register their device in Azure AD, if they haven't already done so.</span></span>|
|<span data-ttu-id="6f053-141">исвиевингбефореакцептанцерекуиред</span><span class="sxs-lookup"><span data-stu-id="6f053-141">isViewingBeforeAcceptanceRequired</span></span>|<span data-ttu-id="6f053-142">Boolean</span><span class="sxs-lookup"><span data-stu-id="6f053-142">Boolean</span></span>|<span data-ttu-id="6f053-143">Указывает, должно ли пользователь расширить Соглашение перед принятием.</span><span class="sxs-lookup"><span data-stu-id="6f053-143">Indicates whether the user has to expand the agreement before accepting.</span></span>|
|<span data-ttu-id="6f053-144">termsExpiration</span><span class="sxs-lookup"><span data-stu-id="6f053-144">termsExpiration</span></span>|[<span data-ttu-id="6f053-145">termsExpiration</span><span class="sxs-lookup"><span data-stu-id="6f053-145">termsExpiration</span></span>](termsexpiration.md)| <span data-ttu-id="6f053-146">Расписание истечения срока действия и периодичность соглашения для всех пользователей.</span><span class="sxs-lookup"><span data-stu-id="6f053-146">Expiration schedule and frequency of agreement for all users.</span></span> |
|<span data-ttu-id="6f053-147">userReacceptRequiredFrequency</span><span class="sxs-lookup"><span data-stu-id="6f053-147">userReacceptRequiredFrequency</span></span>|<span data-ttu-id="6f053-148">Длительность</span><span class="sxs-lookup"><span data-stu-id="6f053-148">Duration</span></span>|<span data-ttu-id="6f053-149">Срок действия, по истечении которого пользователь должен повторно принять условия использования.</span><span class="sxs-lookup"><span data-stu-id="6f053-149">The duration after which the user must re-accept the terms of use.</span></span> <span data-ttu-id="6f053-150">Значение представляется в формате ISO 8601 для длительности.</span><span class="sxs-lookup"><span data-stu-id="6f053-150">The value is represented in ISO 8601 format for durations.</span></span>|


## <a name="relationships"></a><span data-ttu-id="6f053-151">Отношения</span><span class="sxs-lookup"><span data-stu-id="6f053-151">Relationships</span></span>
| <span data-ttu-id="6f053-152">Связь</span><span class="sxs-lookup"><span data-stu-id="6f053-152">Relationship</span></span> | <span data-ttu-id="6f053-153">Тип</span><span class="sxs-lookup"><span data-stu-id="6f053-153">Type</span></span>        | <span data-ttu-id="6f053-154">Описание</span><span class="sxs-lookup"><span data-stu-id="6f053-154">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="6f053-155">приемы</span><span class="sxs-lookup"><span data-stu-id="6f053-155">acceptances</span></span>|<span data-ttu-id="6f053-156">Коллекция [agreementAcceptance](agreementacceptance.md)</span><span class="sxs-lookup"><span data-stu-id="6f053-156">[agreementAcceptance](agreementacceptance.md) collection</span></span>|<span data-ttu-id="6f053-157">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="6f053-157">Read-only.</span></span> <span data-ttu-id="6f053-158">Сведения о приемках настоящего соглашения.</span><span class="sxs-lookup"><span data-stu-id="6f053-158">Information about acceptances of this agreement.</span></span>|
|<span data-ttu-id="6f053-159">files</span><span class="sxs-lookup"><span data-stu-id="6f053-159">files</span></span>|<span data-ttu-id="6f053-160">Коллекция [агриментфилелокализатион](agreementfilelocalization.md)</span><span class="sxs-lookup"><span data-stu-id="6f053-160">[agreementFileLocalization](agreementfilelocalization.md) collection</span></span>| <span data-ttu-id="6f053-161">Документы PDF, связанные с этим соглашением.</span><span class="sxs-lookup"><span data-stu-id="6f053-161">PDFs linked to this agreement.</span></span> <span data-ttu-id="6f053-162">**Примечание:** Это свойство является устаревшим.</span><span class="sxs-lookup"><span data-stu-id="6f053-162">**Note:** This property is in the process of being deprecated.</span></span> <span data-ttu-id="6f053-163">Вместо этого свойству  **файла** усесе.</span><span class="sxs-lookup"><span data-stu-id="6f053-163">Usethe  **file** property instead.</span></span>|
|<span data-ttu-id="6f053-164">file</span><span class="sxs-lookup"><span data-stu-id="6f053-164">file</span></span>|[<span data-ttu-id="6f053-165">agreementFile</span><span class="sxs-lookup"><span data-stu-id="6f053-165">agreementFile</span></span>](agreementfile.md) | <span data-ttu-id="6f053-166">Документы PDF, связанные с этим соглашением.</span><span class="sxs-lookup"><span data-stu-id="6f053-166">PDFs linked to this agreement.</span></span>|


## <a name="json-representation"></a><span data-ttu-id="6f053-167">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="6f053-167">JSON representation</span></span>

<span data-ttu-id="6f053-168">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="6f053-168">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.agreement"
}-->

```json
{
  "id": "String (identifier)",
  "displayName": "MSGraph Sample",
  "isViewingBeforeAcceptanceRequired": true,
  "isPerDeviceAcceptanceRequired": false,
  "termsExpiration": {
    "startDateTime": "2018-10-01T00:00:00.0000000Z",
    "frequency": "PT1M"
  }
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "agreement resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


