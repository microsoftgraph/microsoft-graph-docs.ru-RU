---
title: тип ресурса adminConsentRequestPolicy
description: Указывает политику, с помощью которой можно создавать и управлять запросами на согласие для всего клиента.
author: psignoret
localization_priority: Normal
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 7d7fadabdd8bc3581a2a32b70fad2b27c71c3b5c
ms.sourcegitcommit: 8ca598ac70647bf4f897361ee90d3aa31d2ecca5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/31/2021
ms.locfileid: "51469672"
---
# <a name="adminconsentrequestpolicy-resource-type"></a><span data-ttu-id="cb6f7-103">тип ресурса adminConsentRequestPolicy</span><span class="sxs-lookup"><span data-stu-id="cb6f7-103">adminConsentRequestPolicy resource type</span></span>

<span data-ttu-id="cb6f7-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="cb6f7-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="cb6f7-105">Указывает политику, в которой создаются и управляются запросы на согласие для всего клиента.</span><span class="sxs-lookup"><span data-stu-id="cb6f7-105">Specifies the policy by which consent requests are created and managed for the entire tenant.</span></span> <span data-ttu-id="cb6f7-106">Существует один **администраторConsentRequestPolicy для** каждого клиента.</span><span class="sxs-lookup"><span data-stu-id="cb6f7-106">There is a single **adminConsentRequestPolicy** per tenant.</span></span>

<span data-ttu-id="cb6f7-107">**АдминистраторConsentRequestPolicy** предоставляет дополнительные параметры при создании запроса на согласие, чтобы контролировать поведение функции при запуске запроса на согласие.</span><span class="sxs-lookup"><span data-stu-id="cb6f7-107">The **adminConsentRequestPolicy** provides additional settings when creating a consent request, to control the feature behavior when starting a consent request.</span></span>

## <a name="methods"></a><span data-ttu-id="cb6f7-108">Методы</span><span class="sxs-lookup"><span data-stu-id="cb6f7-108">Methods</span></span>

|<span data-ttu-id="cb6f7-109">Метод</span><span class="sxs-lookup"><span data-stu-id="cb6f7-109">Method</span></span>|<span data-ttu-id="cb6f7-110">Тип возвращаемых данных</span><span class="sxs-lookup"><span data-stu-id="cb6f7-110">Return type</span></span>|<span data-ttu-id="cb6f7-111">Описание</span><span class="sxs-lookup"><span data-stu-id="cb6f7-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="cb6f7-112">Получить adminConsentRequestPolicy</span><span class="sxs-lookup"><span data-stu-id="cb6f7-112">Get adminConsentRequestPolicy</span></span>](../api/adminconsentrequestpolicy-get.md)|[<span data-ttu-id="cb6f7-113">adminConsentRequestPolicy</span><span class="sxs-lookup"><span data-stu-id="cb6f7-113">adminConsentRequestPolicy</span></span>](../resources/adminconsentrequestpolicy.md)|<span data-ttu-id="cb6f7-114">Ознакомьтесь с свойствами и отношениями объекта [adminConsentRequestPolicy.](../resources/adminconsentrequestpolicy.md)</span><span class="sxs-lookup"><span data-stu-id="cb6f7-114">Read the properties and relationships of an [adminConsentRequestPolicy](../resources/adminconsentrequestpolicy.md) object.</span></span>|
|[<span data-ttu-id="cb6f7-115">Обновление adminConsentRequestPolicy</span><span class="sxs-lookup"><span data-stu-id="cb6f7-115">Update adminConsentRequestPolicy</span></span>](../api/adminconsentrequestpolicy-update.md)|[<span data-ttu-id="cb6f7-116">adminConsentRequestPolicy</span><span class="sxs-lookup"><span data-stu-id="cb6f7-116">adminConsentRequestPolicy</span></span>](../resources/adminconsentrequestpolicy.md)|<span data-ttu-id="cb6f7-117">Обновление свойств объекта [adminConsentRequestPolicy.](../resources/adminconsentrequestpolicy.md)</span><span class="sxs-lookup"><span data-stu-id="cb6f7-117">Update the properties of an [adminConsentRequestPolicy](../resources/adminconsentrequestpolicy.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="cb6f7-118">Свойства</span><span class="sxs-lookup"><span data-stu-id="cb6f7-118">Properties</span></span>

|<span data-ttu-id="cb6f7-119">Свойство</span><span class="sxs-lookup"><span data-stu-id="cb6f7-119">Property</span></span>|<span data-ttu-id="cb6f7-120">Тип</span><span class="sxs-lookup"><span data-stu-id="cb6f7-120">Type</span></span>|<span data-ttu-id="cb6f7-121">Описание</span><span class="sxs-lookup"><span data-stu-id="cb6f7-121">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="cb6f7-122">isEnabled</span><span class="sxs-lookup"><span data-stu-id="cb6f7-122">isEnabled</span></span>|<span data-ttu-id="cb6f7-123">Boolean</span><span class="sxs-lookup"><span data-stu-id="cb6f7-123">Boolean</span></span>|<span data-ttu-id="cb6f7-124">Указывает, включена или отключена функция запроса на согласие администратора.</span><span class="sxs-lookup"><span data-stu-id="cb6f7-124">Specifies whether the admin consent request feature is enabled or disabled.</span></span> <span data-ttu-id="cb6f7-125">Обязательное.</span><span class="sxs-lookup"><span data-stu-id="cb6f7-125">Required.</span></span>|
|<span data-ttu-id="cb6f7-126">notifyReviewers</span><span class="sxs-lookup"><span data-stu-id="cb6f7-126">notifyReviewers</span></span>|<span data-ttu-id="cb6f7-127">Логический</span><span class="sxs-lookup"><span data-stu-id="cb6f7-127">Boolean</span></span>|<span data-ttu-id="cb6f7-128">Указывает, будут ли рецензенты получать уведомления.</span><span class="sxs-lookup"><span data-stu-id="cb6f7-128">Specifies whether reviewers will receive notifications.</span></span> <span data-ttu-id="cb6f7-129">Обязательное.</span><span class="sxs-lookup"><span data-stu-id="cb6f7-129">Required.</span></span>|
|<span data-ttu-id="cb6f7-130">remindersEnabled</span><span class="sxs-lookup"><span data-stu-id="cb6f7-130">remindersEnabled</span></span>|<span data-ttu-id="cb6f7-131">Логический</span><span class="sxs-lookup"><span data-stu-id="cb6f7-131">Boolean</span></span>|<span data-ttu-id="cb6f7-132">Указывает, будут ли рецензенты получать сообщения напоминания.</span><span class="sxs-lookup"><span data-stu-id="cb6f7-132">Specifies whether reviewers will receive reminder emails.</span></span> <span data-ttu-id="cb6f7-133">Обязательное.</span><span class="sxs-lookup"><span data-stu-id="cb6f7-133">Required.</span></span>|
|<span data-ttu-id="cb6f7-134">requestDurationInDays</span><span class="sxs-lookup"><span data-stu-id="cb6f7-134">requestDurationInDays</span></span>|<span data-ttu-id="cb6f7-135">Int32</span><span class="sxs-lookup"><span data-stu-id="cb6f7-135">Int32</span></span>|<span data-ttu-id="cb6f7-136">Указывает продолжительность действия запроса до его автоматического истечения, если не будет применено решение.</span><span class="sxs-lookup"><span data-stu-id="cb6f7-136">Specifies the duration the request is active before it automatically expires if no decision is applied.</span></span>|
|<span data-ttu-id="cb6f7-137">рецензенты</span><span class="sxs-lookup"><span data-stu-id="cb6f7-137">reviewers</span></span>|<span data-ttu-id="cb6f7-138">[accessReviewReviewerScope](../resources/accessreviewreviewerscope.md) collection</span><span class="sxs-lookup"><span data-stu-id="cb6f7-138">[accessReviewReviewerScope](../resources/accessreviewreviewerscope.md) collection</span></span>|<span data-ttu-id="cb6f7-139">Список рецензентов для согласия администратора.</span><span class="sxs-lookup"><span data-stu-id="cb6f7-139">The list of reviewers for the admin consent.</span></span> <span data-ttu-id="cb6f7-140">Обязательное.</span><span class="sxs-lookup"><span data-stu-id="cb6f7-140">Required.</span></span>|
|<span data-ttu-id="cb6f7-141">version</span><span class="sxs-lookup"><span data-stu-id="cb6f7-141">version</span></span>|<span data-ttu-id="cb6f7-142">Int32</span><span class="sxs-lookup"><span data-stu-id="cb6f7-142">Int32</span></span>|<span data-ttu-id="cb6f7-143">Указывает версию этой политики.</span><span class="sxs-lookup"><span data-stu-id="cb6f7-143">Specifies the version of this policy.</span></span> <span data-ttu-id="cb6f7-144">Когда политика обновляется, эта версия обновляется.</span><span class="sxs-lookup"><span data-stu-id="cb6f7-144">When the policy is updated, this version is updated.</span></span> <span data-ttu-id="cb6f7-145">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="cb6f7-145">Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="cb6f7-146">Связи</span><span class="sxs-lookup"><span data-stu-id="cb6f7-146">Relationships</span></span>

<span data-ttu-id="cb6f7-147">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="cb6f7-147">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="cb6f7-148">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="cb6f7-148">JSON representation</span></span>

<span data-ttu-id="cb6f7-149">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="cb6f7-149">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.adminConsentRequestPolicy",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.adminConsentRequestPolicy",
  "isEnabled": "Boolean",
  "version": "Integer",
  "notifyReviewers": "Boolean",
  "remindersEnabled": "Boolean",
  "requestDurationInDays": "Integer",
  "reviewers": [
    {
      "@odata.type": "microsoft.graph.accessReviewReviewerScope"
    }
  ]
}
```

