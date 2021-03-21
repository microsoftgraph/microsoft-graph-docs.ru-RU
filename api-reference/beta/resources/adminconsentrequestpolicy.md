---
title: тип ресурса adminConsentRequestPolicy
description: Указывает политику, с помощью которой можно создавать и управлять запросами на согласие для всего клиента.
author: psignoret
localization_priority: Normal
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: dde04ac8c94f0f924df47f3b9490b09f18490c2c
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/20/2021
ms.locfileid: "50965238"
---
# <a name="adminconsentrequestpolicy-resource-type"></a><span data-ttu-id="39ce9-103">тип ресурса adminConsentRequestPolicy</span><span class="sxs-lookup"><span data-stu-id="39ce9-103">adminConsentRequestPolicy resource type</span></span>

<span data-ttu-id="39ce9-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="39ce9-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="39ce9-105">Указывает политику, в которой создаются и управляются запросы на согласие для всего клиента.</span><span class="sxs-lookup"><span data-stu-id="39ce9-105">Specifies the policy by which consent requests are created and managed for the entire tenant.</span></span> <span data-ttu-id="39ce9-106">Существует один **администраторConsentRequestPolicy для** каждого клиента.</span><span class="sxs-lookup"><span data-stu-id="39ce9-106">There is a single **adminConsentRequestPolicy** per tenant.</span></span> 

<span data-ttu-id="39ce9-107">**АдминистраторConsentRequestPolicy** предоставляет дополнительные параметры при создании запроса на согласие, чтобы контролировать поведение функции при запуске запроса на согласие.</span><span class="sxs-lookup"><span data-stu-id="39ce9-107">The **adminConsentRequestPolicy** provides additional settings when creating a consent request, to control the feature behavior when starting a consent request.</span></span>

## <a name="methods"></a><span data-ttu-id="39ce9-108">Методы</span><span class="sxs-lookup"><span data-stu-id="39ce9-108">Methods</span></span>
|<span data-ttu-id="39ce9-109">Метод</span><span class="sxs-lookup"><span data-stu-id="39ce9-109">Method</span></span>|<span data-ttu-id="39ce9-110">Тип возвращаемых данных</span><span class="sxs-lookup"><span data-stu-id="39ce9-110">Return type</span></span>|<span data-ttu-id="39ce9-111">Описание</span><span class="sxs-lookup"><span data-stu-id="39ce9-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="39ce9-112">Получить adminConsentRequestPolicy</span><span class="sxs-lookup"><span data-stu-id="39ce9-112">Get adminConsentRequestPolicy</span></span>](../api/adminconsentrequestpolicy-get.md)|[<span data-ttu-id="39ce9-113">adminConsentRequestPolicy</span><span class="sxs-lookup"><span data-stu-id="39ce9-113">adminConsentRequestPolicy</span></span>](../resources/adminconsentrequestpolicy.md)|<span data-ttu-id="39ce9-114">Ознакомьтесь с свойствами и отношениями объекта [adminConsentRequestPolicy.](../resources/adminconsentrequestpolicy.md)</span><span class="sxs-lookup"><span data-stu-id="39ce9-114">Read the properties and relationships of an [adminConsentRequestPolicy](../resources/adminconsentrequestpolicy.md) object.</span></span>|
|[<span data-ttu-id="39ce9-115">Обновление adminConsentRequestPolicy</span><span class="sxs-lookup"><span data-stu-id="39ce9-115">Update adminConsentRequestPolicy</span></span>](../api/adminconsentrequestpolicy-update.md)|[<span data-ttu-id="39ce9-116">adminConsentRequestPolicy</span><span class="sxs-lookup"><span data-stu-id="39ce9-116">adminConsentRequestPolicy</span></span>](../resources/adminconsentrequestpolicy.md)|<span data-ttu-id="39ce9-117">Обновление свойств объекта [adminConsentRequestPolicy.](../resources/adminconsentrequestpolicy.md)</span><span class="sxs-lookup"><span data-stu-id="39ce9-117">Update the properties of an [adminConsentRequestPolicy](../resources/adminconsentrequestpolicy.md) object.</span></span>|


## <a name="properties"></a><span data-ttu-id="39ce9-118">Свойства</span><span class="sxs-lookup"><span data-stu-id="39ce9-118">Properties</span></span>
|<span data-ttu-id="39ce9-119">Свойство</span><span class="sxs-lookup"><span data-stu-id="39ce9-119">Property</span></span>|<span data-ttu-id="39ce9-120">Тип</span><span class="sxs-lookup"><span data-stu-id="39ce9-120">Type</span></span>|<span data-ttu-id="39ce9-121">Описание</span><span class="sxs-lookup"><span data-stu-id="39ce9-121">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="39ce9-122">isEnabled</span><span class="sxs-lookup"><span data-stu-id="39ce9-122">isEnabled</span></span>|<span data-ttu-id="39ce9-123">Boolean</span><span class="sxs-lookup"><span data-stu-id="39ce9-123">Boolean</span></span>|<span data-ttu-id="39ce9-124">Указывает, включена или отключена функция запроса на согласие администратора.</span><span class="sxs-lookup"><span data-stu-id="39ce9-124">Specifies whether the admin consent request feature is enabled or disabled.</span></span> <span data-ttu-id="39ce9-125">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="39ce9-125">Required.</span></span>|
|<span data-ttu-id="39ce9-126">notifyReviewers</span><span class="sxs-lookup"><span data-stu-id="39ce9-126">notifyReviewers</span></span>|<span data-ttu-id="39ce9-127">Boolean</span><span class="sxs-lookup"><span data-stu-id="39ce9-127">Boolean</span></span>|<span data-ttu-id="39ce9-128">Указывает, будут ли рецензенты получать уведомления.</span><span class="sxs-lookup"><span data-stu-id="39ce9-128">Specifies whether reviewers will receive notifications.</span></span> <span data-ttu-id="39ce9-129">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="39ce9-129">Required.</span></span>|
|<span data-ttu-id="39ce9-130">remindersEnabled</span><span class="sxs-lookup"><span data-stu-id="39ce9-130">remindersEnabled</span></span>|<span data-ttu-id="39ce9-131">Boolean</span><span class="sxs-lookup"><span data-stu-id="39ce9-131">Boolean</span></span>|<span data-ttu-id="39ce9-132">Указывает, будут ли рецензенты получать сообщения напоминания.</span><span class="sxs-lookup"><span data-stu-id="39ce9-132">Specifies whether reviewers will receive reminder emails.</span></span> <span data-ttu-id="39ce9-133">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="39ce9-133">Required.</span></span>|
|<span data-ttu-id="39ce9-134">requestDurationInDays</span><span class="sxs-lookup"><span data-stu-id="39ce9-134">requestDurationInDays</span></span>|<span data-ttu-id="39ce9-135">Int32</span><span class="sxs-lookup"><span data-stu-id="39ce9-135">Int32</span></span>|<span data-ttu-id="39ce9-136">Указывает продолжительность действия запроса до его автоматического истечения, если не будет применено решение.</span><span class="sxs-lookup"><span data-stu-id="39ce9-136">Specifies the duration the request is active before it automatically expires if no decision is applied.</span></span>|
|<span data-ttu-id="39ce9-137">рецензенты</span><span class="sxs-lookup"><span data-stu-id="39ce9-137">reviewers</span></span>|<span data-ttu-id="39ce9-138">[accessReviewReviewerScope](../resources/accessreviewreviewerscope.md) collection</span><span class="sxs-lookup"><span data-stu-id="39ce9-138">[accessReviewReviewerScope](../resources/accessreviewreviewerscope.md) collection</span></span>|<span data-ttu-id="39ce9-139">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="39ce9-139">Required.</span></span>|
|<span data-ttu-id="39ce9-140">version</span><span class="sxs-lookup"><span data-stu-id="39ce9-140">version</span></span>|<span data-ttu-id="39ce9-141">Int32</span><span class="sxs-lookup"><span data-stu-id="39ce9-141">Int32</span></span>|<span data-ttu-id="39ce9-142">Указывает версию этой политики.</span><span class="sxs-lookup"><span data-stu-id="39ce9-142">Specifies the version of this policy.</span></span> <span data-ttu-id="39ce9-143">Когда политика обновляется, эта версия обновляется.</span><span class="sxs-lookup"><span data-stu-id="39ce9-143">When the policy is updated, this version is updated.</span></span> <span data-ttu-id="39ce9-144">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="39ce9-144">Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="39ce9-145">Связи</span><span class="sxs-lookup"><span data-stu-id="39ce9-145">Relationships</span></span>
<span data-ttu-id="39ce9-146">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="39ce9-146">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="39ce9-147">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="39ce9-147">JSON representation</span></span>
<span data-ttu-id="39ce9-148">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="39ce9-148">The following is a JSON representation of the resource.</span></span>
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
