---
title: тип перечисления Фиреваллпрешаредкэйенкодингмесодтипе
description: Возможные значения для Фиреваллпрешаредкэйенкодингмесод
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: a563d030a12480c6151a76cf2d58f743783bb378
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36031544"
---
# <a name="firewallpresharedkeyencodingmethodtype-enum-type"></a><span data-ttu-id="cf2a7-103">тип перечисления Фиреваллпрешаредкэйенкодингмесодтипе</span><span class="sxs-lookup"><span data-stu-id="cf2a7-103">firewallPreSharedKeyEncodingMethodType enum type</span></span>

> <span data-ttu-id="cf2a7-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="cf2a7-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="cf2a7-105">Возможные значения для Фиреваллпрешаредкэйенкодингмесод</span><span class="sxs-lookup"><span data-stu-id="cf2a7-105">Possible values for firewallPreSharedKeyEncodingMethod</span></span>

## <a name="members"></a><span data-ttu-id="cf2a7-106">Элементы</span><span class="sxs-lookup"><span data-stu-id="cf2a7-106">Members</span></span>
|<span data-ttu-id="cf2a7-107">Элемент</span><span class="sxs-lookup"><span data-stu-id="cf2a7-107">Member</span></span>|<span data-ttu-id="cf2a7-108">Значение</span><span class="sxs-lookup"><span data-stu-id="cf2a7-108">Value</span></span>|<span data-ttu-id="cf2a7-109">Описание</span><span class="sxs-lookup"><span data-stu-id="cf2a7-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="cf2a7-110">Девицедефаулт</span><span class="sxs-lookup"><span data-stu-id="cf2a7-110">deviceDefault</span></span>|<span data-ttu-id="cf2a7-111">нуль</span><span class="sxs-lookup"><span data-stu-id="cf2a7-111">0</span></span>|<span data-ttu-id="cf2a7-112">Значение не настроено Intune, не переопределять значение устройства по умолчанию, настроенное пользователем</span><span class="sxs-lookup"><span data-stu-id="cf2a7-112">No value configured by Intune, do not override the user-configured device default value</span></span>|
|<span data-ttu-id="cf2a7-113">none</span><span class="sxs-lookup"><span data-stu-id="cf2a7-113">none</span></span>|<span data-ttu-id="cf2a7-114">1,1</span><span class="sxs-lookup"><span data-stu-id="cf2a7-114">1</span></span>|<span data-ttu-id="cf2a7-115">Общий ключ не кодируется.</span><span class="sxs-lookup"><span data-stu-id="cf2a7-115">Preshared key is not encoded.</span></span> <span data-ttu-id="cf2a7-116">Вместо этого он хранится в расширенном формате символов</span><span class="sxs-lookup"><span data-stu-id="cf2a7-116">Instead, it is kept in its wide-character format</span></span>|
|<span data-ttu-id="cf2a7-117">utF8</span><span class="sxs-lookup"><span data-stu-id="cf2a7-117">utF8</span></span>|<span data-ttu-id="cf2a7-118">2</span><span class="sxs-lookup"><span data-stu-id="cf2a7-118">2</span></span>|<span data-ttu-id="cf2a7-119">Кодирование общего ключа с помощью UTF – 8</span><span class="sxs-lookup"><span data-stu-id="cf2a7-119">Encode the preshared key using UTF-8</span></span>|



