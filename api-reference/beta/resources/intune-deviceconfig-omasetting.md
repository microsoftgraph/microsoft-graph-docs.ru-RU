---
title: Тип ресурса omaSetting
description: Определение параметра OMA.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: e05111209d50fec1aee52a5e9ee87baae3ca47a1
ms.sourcegitcommit: ed45b5ce0583dfa4d12f7cb0b3ac0c5aeb2318d4
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/16/2021
ms.locfileid: "51867450"
---
# <a name="omasetting-resource-type"></a><span data-ttu-id="ced77-103">Тип ресурса omaSetting</span><span class="sxs-lookup"><span data-stu-id="ced77-103">omaSetting resource type</span></span>

<span data-ttu-id="ced77-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ced77-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="ced77-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ced77-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ced77-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="ced77-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ced77-107">Определение параметра OMA.</span><span class="sxs-lookup"><span data-stu-id="ced77-107">OMA Settings definition.</span></span>

## <a name="properties"></a><span data-ttu-id="ced77-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="ced77-108">Properties</span></span>
|<span data-ttu-id="ced77-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="ced77-109">Property</span></span>|<span data-ttu-id="ced77-110">Тип</span><span class="sxs-lookup"><span data-stu-id="ced77-110">Type</span></span>|<span data-ttu-id="ced77-111">Описание</span><span class="sxs-lookup"><span data-stu-id="ced77-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ced77-112">displayName</span><span class="sxs-lookup"><span data-stu-id="ced77-112">displayName</span></span>|<span data-ttu-id="ced77-113">String</span><span class="sxs-lookup"><span data-stu-id="ced77-113">String</span></span>|<span data-ttu-id="ced77-114">Отображаемое имя.</span><span class="sxs-lookup"><span data-stu-id="ced77-114">Display Name.</span></span>|
|<span data-ttu-id="ced77-115">description</span><span class="sxs-lookup"><span data-stu-id="ced77-115">description</span></span>|<span data-ttu-id="ced77-116">String</span><span class="sxs-lookup"><span data-stu-id="ced77-116">String</span></span>|<span data-ttu-id="ced77-117">Описание.</span><span class="sxs-lookup"><span data-stu-id="ced77-117">Description.</span></span>|
|<span data-ttu-id="ced77-118">omaUri</span><span class="sxs-lookup"><span data-stu-id="ced77-118">omaUri</span></span>|<span data-ttu-id="ced77-119">String</span><span class="sxs-lookup"><span data-stu-id="ced77-119">String</span></span>|<span data-ttu-id="ced77-120">OMA.</span><span class="sxs-lookup"><span data-stu-id="ced77-120">OMA.</span></span>|
|<span data-ttu-id="ced77-121">secretReferenceValueId</span><span class="sxs-lookup"><span data-stu-id="ced77-121">secretReferenceValueId</span></span>|<span data-ttu-id="ced77-122">String</span><span class="sxs-lookup"><span data-stu-id="ced77-122">String</span></span>|<span data-ttu-id="ced77-123">ReferenceId для поисков секрета для расшифровки.</span><span class="sxs-lookup"><span data-stu-id="ced77-123">ReferenceId for looking up secret for decryption.</span></span> <span data-ttu-id="ced77-124">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="ced77-124">This property is read-only.</span></span>|
|<span data-ttu-id="ced77-125">isEncrypted</span><span class="sxs-lookup"><span data-stu-id="ced77-125">isEncrypted</span></span>|<span data-ttu-id="ced77-126">Boolean</span><span class="sxs-lookup"><span data-stu-id="ced77-126">Boolean</span></span>|<span data-ttu-id="ced77-127">Указывает, зашифровано ли поле значений.</span><span class="sxs-lookup"><span data-stu-id="ced77-127">Indicates whether the value field is encrypted.</span></span> <span data-ttu-id="ced77-128">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="ced77-128">This property is read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="ced77-129">Связи</span><span class="sxs-lookup"><span data-stu-id="ced77-129">Relationships</span></span>
<span data-ttu-id="ced77-130">Нет</span><span class="sxs-lookup"><span data-stu-id="ced77-130">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="ced77-131">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="ced77-131">JSON Representation</span></span>
<span data-ttu-id="ced77-132">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="ced77-132">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.omaSetting"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.omaSetting",
  "displayName": "String",
  "description": "String",
  "omaUri": "String",
  "secretReferenceValueId": "String",
  "isEncrypted": true
}
```




