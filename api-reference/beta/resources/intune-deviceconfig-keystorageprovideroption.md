---
title: Тип перечисления keyStorageProviderOption
description: Параметры импорта хранилища ключей поставщика (поставщика хранилища КЛЮЧЕЙ).
author: tfitzmac
ms.openlocfilehash: 7923dd5c4b8a09d834d29b65928430828f3dafac
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27342219"
---
# <a name="keystorageprovideroption-enum-type"></a>Тип перечисления keyStorageProviderOption

> **Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается.

> **Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.

Параметры импорта хранилища ключей поставщика (поставщика хранилища КЛЮЧЕЙ).
## <a name="members"></a>Элементы
|Элемент|Значение|Описание|
|:---|:---|:---|
|useTpmKspOtherwiseUseSoftwareKsp|0|Импорта для доверенного платформы модуля (TPM) поставщика хранилища КЛЮЧЕЙ, если этот параметр указан, в противном случае — импорт поставщика хранилища КЛЮЧЕЙ программного обеспечения.|
|useTpmKspOtherwiseFail|1|Импорт для доверенного платформы модуля (TPM) поставщика хранилища КЛЮЧЕЙ, если этот параметр указан, в противном случае — не удается.|
|usePassportForWorkKspOtherwiseFail|2|Импорт Passport для работы поставщика хранилища КЛЮЧЕЙ Если доступно, в противном случае — ошибка.|
|useSoftwareKsp|3|Импорт на программное обеспечение поставщика хранилища КЛЮЧЕЙ.|





