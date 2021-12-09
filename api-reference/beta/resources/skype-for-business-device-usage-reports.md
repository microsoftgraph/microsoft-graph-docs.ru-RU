---
title: Отчеты об использовании устройств со Skype для бизнеса
description: Вы можете получить сведения о типах клиентов и устройств, используемых в организации. Эти данные могут пригодиться при проведении анализа, планировании и принятии других бизнес-решений для организации.
ms.localizationpriority: medium
ms.prod: reports
author: sarahwxy
doc_type: conceptualPageType
ms.openlocfilehash: c899974dfe42117a6a1ef2dd20a957fcb6f832f3
ms.sourcegitcommit: f336c5c49fbcebe55312656aa8b50511fd99a657
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/09/2021
ms.locfileid: "61390866"
---
# <a name="skype-for-business-device-usage-reports"></a>Отчеты об использовании устройств со Skype для бизнеса

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Вы можете получить сведения о типах клиентов и устройств, используемых в организации. Эти данные могут пригодиться при проведении анализа, планировании и принятии других бизнес-решений для организации.

> **Примечание:** Подробные сведения о различных представлениях отчетов и [именах см. в Microsoft 365 отчетов — Skype для бизнеса используемых клиентов.](https://support.office.com/client/Skype-for-Business-clients-used-b9019c36-034f-40c7-acb0-c2a0400b03c3)

## <a name="reports"></a>Отчеты

| Функция                                                     | Тип возврата CSV | Тип возврата JSON | Описание                                                  |
| :----------------------------------------------------------- | :-------------- | :--------------- | ------------------------------------------------------------ |
| [Получение сведений о пользователях](../api/reportroot-getskypeforbusinessdeviceusageuserdetail.md) | Stream          | Stream           | Получите сведения об использовании устройств со Skype для бизнеса с разбивкой по пользователям.   |
| [Получение количества пользователей с разбивкой по устройствам](../api/reportroot-getskypeforbusinessdeviceusagedistributionusercounts.md) | Stream          | Stream           | Узнайте, сколько сотрудников организации используют уникальные устройства. В отчете будет показано количество пользователей устройств с Windows, телефонов с Windows, телефонов с Android, iPhone и iPad. |
| [Получение количества пользователей](../api/reportroot-getskypeforbusinessdeviceusageusercounts.md) | Stream          | Stream           | Отследите динамику использования по количеству пользователей в организации, подключавшихся с помощью приложения Skype для бизнеса. Кроме того, вы получите статистические данные с разбивкой по типу устройства (устройство с Windows, телефон с Windows, телефон с Android, iPhone или iPad), на котором установлено клиентское приложение Skype для бизнеса, используемое в организации. |


