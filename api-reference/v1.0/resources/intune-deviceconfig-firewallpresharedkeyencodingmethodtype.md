---
title: тип перечисления Фиреваллпрешаредкэйенкодингмесодтипе
description: Возможные значения для Фиреваллпрешаредкэйенкодингмесод
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 07ea8e7a3a5622446ab2c0126d21187f6d7ce3b9
ms.sourcegitcommit: bd5bb20856d4bffe93b2f77f131664849b602dbb
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/02/2019
ms.locfileid: "37359238"
---
# <a name="firewallpresharedkeyencodingmethodtype-enum-type"></a><span data-ttu-id="050d1-103">тип перечисления Фиреваллпрешаредкэйенкодингмесодтипе</span><span class="sxs-lookup"><span data-stu-id="050d1-103">firewallPreSharedKeyEncodingMethodType enum type</span></span>

> <span data-ttu-id="050d1-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="050d1-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="050d1-105">Возможные значения для Фиреваллпрешаредкэйенкодингмесод</span><span class="sxs-lookup"><span data-stu-id="050d1-105">Possible values for firewallPreSharedKeyEncodingMethod</span></span>

## <a name="members"></a><span data-ttu-id="050d1-106">Элементы</span><span class="sxs-lookup"><span data-stu-id="050d1-106">Members</span></span>
|<span data-ttu-id="050d1-107">Элемент</span><span class="sxs-lookup"><span data-stu-id="050d1-107">Member</span></span>|<span data-ttu-id="050d1-108">Значение</span><span class="sxs-lookup"><span data-stu-id="050d1-108">Value</span></span>|<span data-ttu-id="050d1-109">Описание</span><span class="sxs-lookup"><span data-stu-id="050d1-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="050d1-110">девицедефаулт</span><span class="sxs-lookup"><span data-stu-id="050d1-110">deviceDefault</span></span>|<span data-ttu-id="050d1-111">нуль</span><span class="sxs-lookup"><span data-stu-id="050d1-111">0</span></span>|<span data-ttu-id="050d1-112">Значение не настроено Intune, не переопределять значение устройства по умолчанию, настроенное пользователем</span><span class="sxs-lookup"><span data-stu-id="050d1-112">No value configured by Intune, do not override the user-configured device default value</span></span>|
|<span data-ttu-id="050d1-113">none</span><span class="sxs-lookup"><span data-stu-id="050d1-113">none</span></span>|<span data-ttu-id="050d1-114">1,1</span><span class="sxs-lookup"><span data-stu-id="050d1-114">1</span></span>|<span data-ttu-id="050d1-115">Общий ключ не кодируется.</span><span class="sxs-lookup"><span data-stu-id="050d1-115">Preshared key is not encoded.</span></span> <span data-ttu-id="050d1-116">Вместо этого он хранится в расширенном формате символов</span><span class="sxs-lookup"><span data-stu-id="050d1-116">Instead, it is kept in its wide-character format</span></span>|
|<span data-ttu-id="050d1-117">utF8</span><span class="sxs-lookup"><span data-stu-id="050d1-117">utF8</span></span>|<span data-ttu-id="050d1-118">2</span><span class="sxs-lookup"><span data-stu-id="050d1-118">2</span></span>|<span data-ttu-id="050d1-119">Кодирование общего ключа с помощью UTF – 8</span><span class="sxs-lookup"><span data-stu-id="050d1-119">Encode the preshared key using UTF-8</span></span>|




