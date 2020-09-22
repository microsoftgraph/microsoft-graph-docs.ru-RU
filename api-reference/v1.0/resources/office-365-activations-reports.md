---
title: Отчеты об активации Microsoft 365
description: Отчеты об активации Microsoft 365 могут предоставить представление о том, какие пользователи активировали подписки Microsoft 365 по крайней мере на одном устройстве. В этих отчетах представлены сведения об активации подписки на Microsoft 365 профессиональный плюс, Project и Visio Pro для Office 365, а также разделение активаций на настольных компьютерах и устройствах. Эти отчеты помогут вам выявить пользователей, которым, возможно, нужна помощь с активацией подписки на Office.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: conceptualPageType
ms.openlocfilehash: ebca76ca3fe9356839636e7dca29293b083c13ff
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "47970672"
---
# <a name="microsoft-365-activations-reports"></a>Отчеты об активации Microsoft 365

Пространство имен: microsoft.graph

Отчеты об активации Microsoft 365 могут предоставить представление о том, какие пользователи активировали подписки Microsoft 365 по крайней мере на одном устройстве. В этих отчетах представлены сведения об активации подписки на Microsoft 365 профессиональный плюс, Project и Visio Pro для Office 365, а также разделение активаций на настольных компьютерах и устройствах. Эти отчеты помогут вам выявить пользователей, которым, возможно, нужна помощь с активацией подписки на Office.

> **Примечание:** Сведения о различных представлениях отчетов и их именах можно найти в [статье Microsoft 365 Reports — активации Microsoft Office](https://support.office.com/client/Office-activations-87c24ae2-82e0-4d1e-be01-c3bcc3f18c60).

## <a name="reports"></a>Отчеты
| Функция                                 | Возвращаемый тип | Описание                              |
| :--------------------------------------- | :---------- | :--------------------------------------- |
| [Получение сведений о пользователях](../api/reportroot-getoffice365activationsuserdetail.md) | Stream      | Получение сведений о пользователях, которые активировали Microsoft 365. |
| [Получение количества активаций](../api/reportroot-getoffice365activationcounts.md) | Поток      | Получение числа активаций Microsoft 365 на настольных компьютерах и устройствах. |
| [Получение количества пользователей](../api/reportroot-getoffice365activationsusercounts.md) | Stream      | Узнайте, сколько пользователей активировали подписку на Office на компьютере или мобильном устройстве. |

