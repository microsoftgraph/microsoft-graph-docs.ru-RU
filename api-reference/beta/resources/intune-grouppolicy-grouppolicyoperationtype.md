---
title: тип перечисления Граупполициоператионтипе
description: Тип операции с групповой политикой.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: fece2bafc46dbc4c5d7019fbf4b4cacd8f2330ac
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48030964"
---
# <a name="grouppolicyoperationtype-enum-type"></a><span data-ttu-id="1a694-103">тип перечисления Граупполициоператионтипе</span><span class="sxs-lookup"><span data-stu-id="1a694-103">groupPolicyOperationType enum type</span></span>

<span data-ttu-id="1a694-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1a694-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="1a694-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1a694-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="1a694-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="1a694-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1a694-107">Тип операции с групповой политикой.</span><span class="sxs-lookup"><span data-stu-id="1a694-107">Type of Group Policy operation.</span></span>

## <a name="members"></a><span data-ttu-id="1a694-108">Элементы</span><span class="sxs-lookup"><span data-stu-id="1a694-108">Members</span></span>
|<span data-ttu-id="1a694-109">Элемент</span><span class="sxs-lookup"><span data-stu-id="1a694-109">Member</span></span>|<span data-ttu-id="1a694-110">Значение</span><span class="sxs-lookup"><span data-stu-id="1a694-110">Value</span></span>|<span data-ttu-id="1a694-111">Описание</span><span class="sxs-lookup"><span data-stu-id="1a694-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1a694-112">Нет</span><span class="sxs-lookup"><span data-stu-id="1a694-112">none</span></span>|<span data-ttu-id="1a694-113">нуль</span><span class="sxs-lookup"><span data-stu-id="1a694-113">0</span></span>|<span data-ttu-id="1a694-114">Групповая политика: недопустимый тип операции.</span><span class="sxs-lookup"><span data-stu-id="1a694-114">Group Policy invalid operation type.</span></span>|
|<span data-ttu-id="1a694-115">загрузку</span><span class="sxs-lookup"><span data-stu-id="1a694-115">upload</span></span>|<span data-ttu-id="1a694-116">1 </span><span class="sxs-lookup"><span data-stu-id="1a694-116">1</span></span>|<span data-ttu-id="1a694-117">Тип операции отправки групповой политики.</span><span class="sxs-lookup"><span data-stu-id="1a694-117">Group Policy upload operation type.</span></span>|
|<span data-ttu-id="1a694-118">уплоадневверсион</span><span class="sxs-lookup"><span data-stu-id="1a694-118">uploadNewVersion</span></span>|<span data-ttu-id="1a694-119">2 </span><span class="sxs-lookup"><span data-stu-id="1a694-119">2</span></span>|<span data-ttu-id="1a694-120">Отправка типа операции новой версии групповой политики.</span><span class="sxs-lookup"><span data-stu-id="1a694-120">Group Policy upload new version operation type.</span></span>|
|<span data-ttu-id="1a694-121">аддлангуажефилес</span><span class="sxs-lookup"><span data-stu-id="1a694-121">addLanguageFiles</span></span>|<span data-ttu-id="1a694-122">4</span><span class="sxs-lookup"><span data-stu-id="1a694-122">3</span></span>|<span data-ttu-id="1a694-123">Тип операции "Добавление файлов нового языка" групповой политики (ADML).</span><span class="sxs-lookup"><span data-stu-id="1a694-123">Group Policy add new language(ADML) files operation type.</span></span>|
|<span data-ttu-id="1a694-124">ремовелангуажефилес</span><span class="sxs-lookup"><span data-stu-id="1a694-124">removeLanguageFiles</span></span>|<span data-ttu-id="1a694-125">4 </span><span class="sxs-lookup"><span data-stu-id="1a694-125">4</span></span>|<span data-ttu-id="1a694-126">Тип операции удаления файлов на языке групповой политики (ADML).</span><span class="sxs-lookup"><span data-stu-id="1a694-126">Group Policy remove language(ADML) files operation type.</span></span>|
|<span data-ttu-id="1a694-127">упдателангуажефилес</span><span class="sxs-lookup"><span data-stu-id="1a694-127">updateLanguageFiles</span></span>|<span data-ttu-id="1a694-128">5 </span><span class="sxs-lookup"><span data-stu-id="1a694-128">5</span></span>|<span data-ttu-id="1a694-129">Тип операции для файлов на языке обновлений групповой политики (ADML).</span><span class="sxs-lookup"><span data-stu-id="1a694-129">Group Policy update language(ADML) files operation type.</span></span>|
|<span data-ttu-id="1a694-130">удалить</span><span class="sxs-lookup"><span data-stu-id="1a694-130">remove</span></span>|<span data-ttu-id="1a694-131">6 </span><span class="sxs-lookup"><span data-stu-id="1a694-131">6</span></span>|<span data-ttu-id="1a694-132">Групповая политика удалить отправленный тип операции с файлами.</span><span class="sxs-lookup"><span data-stu-id="1a694-132">Group Policy remove uploaded file operation type.</span></span>|






